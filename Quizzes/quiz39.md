## Code on Python
```.py
from kivymd.app import MDApp

class quiz39(MDApp):
    def __init__(self):
        super().__init__()
        self.count = 0
    def build(self):
        return
    def increase(self):
        self.count += 1
        self.root.ids.my_label.text = f"Count {self.count}"
m = quiz39()
m.run()
```
## kv file
```.kv
Screen:
    size:500,500 #width, height
    MDBoxLayout:
        orientation: "horizontal"
        size_hint: 0.7, 0.3 #percentages of the screen
        pos_hint:{"center_x":0.5, "center_y":0.5}
        MDLabel:
            id: my_label
            halign: "center"
            size_hint: 0.5, 1
            text: "Count "
            font_size: 34
        MDRaisedButton:
            id: my_button
            text: "Add+1"
            md_bg_color: 0,1,1,1
            size_hint: 0.5, 1
            pos_hint:{"center_x":0.5, "center_y":0.5}
            font_size: 34
            on_release:
                app.increase()

```

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz39.png)
