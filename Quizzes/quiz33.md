## Code
```.py
import requests

import matplotlib.pyplot as plt
from matplotlib.gridspec import GridSpec


def download(url:str="192.168.6.142/readings")->list:
    plt.style.use("seaborn-v0_8-darkgrid")

    req = requests.get(f'http://{url}')
    data = req.json()
    readings = data["readings"][0]
    return readings

def get_sensor(readings:list, id:int)->list:
    T = []
    for r in readings:
        if r["sensor_id"]==id:
            T.append(r['value'])
    return T

def smoothing(data:list,size_window:int=12):
    x = [] #horizontal axis
    y = [] #smoothed version vertical axis
    for i in range(0, len(data), size_window):
        segment_mean = sum(data[i:i+size_window]) / size_window
        y.append(segment_mean)
        x.append(i)
    return x,y

readings = download()
sensors = [6,8,9,10]

sensor_data = []
for s in sensors:
    data = get_sensor(readings, s)
    x, data_smth = smoothing(data[0:501])
    sensor_data.append(data_smth)

mean_per_hour = []
for i in range(len(sensor_data[0])):
    d = [sensor_data[x][i] for x in range(len(sensors))]
    mean_per_hour.append(sum(d)/len(sensors))

fig = plt.figure(figsize=(10,8))
grid = GridSpec(4,4, figure=fig)
box1 = fig.add_subplot(grid[0:4, 0:3])
plt.plot(x, mean_per_hour, color="#4F000B")
plt.title(f"Mean temperature of sensors {sensors}")
plt.xlabel("Hours")
plt.xlabel("Temp (Celsius)")

my_colors = ["#720026","#CE4257","#FF7F51","#FF9B54"]
for i in range(len(sensors)):
    box2 = fig.add_subplot(grid[i,3])
    plt.plot(x, sensor_data[i], color=my_colors[i])
    plt.title(f"Sensor #{sensors[i]}")
    plt.ylim([20,28])
plt.show()
```
