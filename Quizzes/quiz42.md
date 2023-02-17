# Python code
```.py
from kivymd.app import MDApp
from kivymd.uix.screen import MDScreen

class MysteryPageA(MDScreen):
    pass

class MysteryPageB(MDScreen):
    pass

class quiz42(MDApp):
    def build(self):
        return

test = quiz42()
test.run()
```
# KV file
```.kv
ScreenManager:
    MysteryPageA:
        name:"MysteryPageA"

    MysteryPageB:
        name:"MysteryPageB"

<MysteryPageA>:
    size:500,500
    MDLabel:
        halign: "center"
        text:"This is mystery page A you pressed the button"
    MDRaisedButton:
        pos_hint: {"center_x":.5, "center_y":.4}
        text:"Mystery Page B"
        on_press: root.parent.current = "MysteryPageB"
        md_bg_color: "#e89ec7"



<MysteryPageB>:
    size:500,500
    MDLabel:
        halign: "center"
        text:"This is mystery page B you pressed the button"
    MDRaisedButton:
        pos_hint: {"center_x":.5, "center_y":.4}
        text:"Mystery Page A"
        on_press: root.parent.current = "MysteryPageA"
        md_bg_color: "#e89ec7"
```
# Evidance
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz42_1.png)
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz42_2.png)
