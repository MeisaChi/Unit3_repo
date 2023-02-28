# Python Codes
```.py
class Flight:
    def __init__(self, flight_number:str, origin:str, destination:str, departure_time:str, duration:list):
        self.flight_number = flight_number
        self.origin = origin
        self.destination = destination
        self.departure_time = departure_time
        self.duration = duration

    def get_duration(self)->str:
        hour = self.duration[0]
        min = self.duration[1]
        sec = self.duration[2]
        duration = f"{hour} hours {min} minutes and {sec} seconds"
        return duration

    def get_flightdatas(self)->str:
        flight_number = self.flight_number
        origin = self.origin
        destination = self.destination
        departure_time = self.departure_time
        hour = self.duration[0]
        min = self.duration[1]
        sec = self.duration[2]
        duration = f"Flight number {flight_number}, will depart {origin} at {departure_time}. It will land on {destination} in {hour} hours {min} minutes and {sec} seconds."
        return duration


flight1 = Flight(flight_number="JP567", origin="Japan", destination="New York", departure_time="12:00PM", duration=[12,3,1])
flight2 = Flight(flight_number="LA762", origin="Los Angeles", destination="Hong Kong", departure_time="8:00PM", duration=[21,2,34])

print(flight1.get_duration())
print(flight2.get_duration())
print(flight1.get_flightdatas())
print(flight2.get_flightdatas())
```
# Result
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz50.png)
