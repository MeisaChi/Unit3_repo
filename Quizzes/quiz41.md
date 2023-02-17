# Python code
```.py
from kivymd.app import MDApp


class quiz41(MDApp):
    def build(self):
        return

test = quiz41()
test.run()
```
# KV file
```.kv
Screen:
    size:500,500
    MDBoxLayout:
        id: main_box
        orientation:"vertical"
        size_hint: 0.8, .8
        pos_hint:{"center_x":0.5, "center_y":0.5}
        MDBoxLayout:
            id: first_box
            orientation:"vertical"
            size_hint: 1, .25
            MDLabel:
                text:"TicTacToe by Meisa Chi"
                halign:"center"
            MDLabel:
                text:"It is X's turn"
                halign:"center"
        MDBoxLayout:
            id: second_box
            orientation:"horizontal"
            size_hint: 1, .25
            MDRaisedButton:
                id: left_square
                text: "O"
                size_hint: 1, 1
                md_bg_color: "#fff673"
            MDRaisedButton:
                id: middle_square
                size_hint: 1, 1
                md_bg_color: "#73ff75"
            MDRaisedButton:
                id: right_square
                size_hint: 1, 1
                md_bg_color: "#73ff75"

        MDBoxLayout:
            id: third_box
            orientation:"horizontal"
            size_hint: 1, .25
            MDRaisedButton:
                id: left_square
                text: "X"
                size_hint: 1, 1
                md_bg_color: "#ed686d"
            MDRaisedButton:
                id: middle_square
                size_hint: 1, 1
                md_bg_color: "#73ff75"
            MDRaisedButton:
                id: right_square
                size_hint: 1, 1
                md_bg_color: "#73ff75"

        MDBoxLayout:
            id: fourth_box
            orientation:"horizontal"
            size_hint: 1, .25
            MDRaisedButton:
                id: left_square

                size_hint: 1, 1
                md_bg_color: "#73ff75"
            MDRaisedButton:
                id: middle_square
                size_hint: 1, 1
                md_bg_color: "#73ff75"
            MDRaisedButton:
                id: right_square
                size_hint: 1, 1
```
# Evidance
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz41.png)
