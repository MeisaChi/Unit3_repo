## Code on Python
```.py
from kivymd.app import MDApp

class quiz40(MDApp):
    def build(self):
        return

m = quiz40()
m.run()
```
## kv file
```.kv
Screen:
    size:500,500 #width, height
    md_bg_color: "#ffb5e8"
    MDBoxLayout:
        id: main_box
        orientation:"vertical"
        size_hint: 1, 1
        pos_hint:{"center_x":0.5, "center_y":0.5}

        MDLabel:
            id: Name
            text: "Meisa"
            font_size: 400
            color: "##854155"
            halign: "center"


```

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz40.png)
