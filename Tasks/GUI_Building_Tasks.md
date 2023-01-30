# GUI Building Tasks

### currency_converter.py
```.py
from kivymd.app import MDApp

class currency(MDApp):
    def __init__(self):
        super().__init__()
        self.count = 0

    def build(self):
        return

    def convert_to_jpy(self):
        number = int(self.root.ids.HKD.text)
        self.count = number
        self.root.ids.final_currency.text = f"{self.count*16.57} JPY"

    def convert_to_usd(self):
        number = int(self.root.ids.HKD.text)
        self.count = number
        self.root.ids.final_currency.text = f"{self.count*0.13} USD"

m = currency()
m.run()
```

### currency.kv
```.py
Screen:
    size:500,500 #width, height
    md_bg_color: "#ffb5e8"
    MDBoxLayout:
        id: main_box
        orientation:"vertical"
        size_hint: 0.9, 0.7
        pos_hint:{"center_x":0.5, "center_y":0.5}

        MDLabel:
            id: Currency_converter
            text: "Currency Converter"
            font_size: 80
            color: "#B5C3FF"
            size_hint: 1, 0.2

        MDTextField:
            id: HKD
            hint_text: "Enter an amount in HKD"
            mode:"rectangle"
            size_hint: 1, 0.2
            pos_hint:{"center_x":0.5, "center_y":0.5}

        MDBoxLayout:
            id: second_box
            size_hint: 1, 0.2
            orientation:"horizontal"
            pos_hint:{"center_x":0.5, "center_y":0.5}

            MDLabel:
                id: convert_label
                text: "CLICK TO CONVERT"
                font_size: 50
                color: "#B5C3FF"
                size_hint: 0.6, 0.5

            MDRaisedButton:
                id: jpn
                text: "JPY"
                size_hint: 0.1, 0.5
                color: "#B5FFCC"
                on_release:
                    app.convert_to_jpy()

            MDRaisedButton:
                id: usd
                text: "USD"
                size_hint: 0.1, 0.5
                color: "#FFF1B5"
                on_release:
                    app.convert_to_usd()

        MDBoxLayout:
            id: currency
            orientation:"vertical"
            size_hint: 0.3, 0.3
            pos_hint:{"center_x":1, "center_y":0.5}

            MDLabel:
                id: final_currency
                text: "Amount"
                font_size: 50
                color: "#B5C3FF"
                size_hint: 0.6, 0.5
```
### Converting to JPY
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/converter_1.png)
### Converting to USD
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/converter_2.png)
