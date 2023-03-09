# Unit 3: ISAK Free Store App
## Criteria A: Planning

## Problem definition
**Client:** A student from UWC ISAK Japan

**Context:** UWC ISAK Japan has a free store, where anyone can leave their clothes and other items that they  to give, and anyone can take them for free. But there is so much stuff that it is difficult for the students to look through and check if they want anything from there! A teacher assigned a student in ISAK, who is our client for this program. The client tried everything - requesting for a larger free store, which hadn't worked because there is limited space in ISAK, she also tried sorting out and making the free store more visible, but everyday things were added and taken, that the free store went back to being messy in a week. The client wants a program that she can use on her MacBook which helps her and her schoolmates use the free store efficiently, as there are a lot of good resources there. She wants a well designed software so that it is easy for the students in ISAK to use.


**Problem:** The free store is unorganized, and difficult to use. As the client is a student, she wants the production cost to be as low as possible.


## Proposed Solution

Considering that the student has limited budget to solve the issue, and the context of the problem, the solution that I propose for the client is using Python, KivyMD and SQLite to create a GUI interface.

### Design Statement



I will design a program on Pycharm which will be showing a GUI interface, by using languages : KivyMD, to design the GUI of the App and SQLite, to store the data. To solve the problem, I will be creating a program where the client and their target audiences can use to add items into the free store, look at the items in the free store and take items out of the freestore, on an App. When the client is adding items, they can enter specific datas (category, brand, size, color, description, condition) and that will be available to be shown in a table. The app will also allow require the user to login or create an account to access all the data. When creating the account, their username, password (securely stored) and email will be recorded on a database. This app will take a month (from Feb 10th to March 10th) to develop.

## Justification

### Python
One of the reason I chose Python is because it is one of the fastest-growing languages in the world, as it is considered as one of the best programming languages for machine learning[^1]. Python runs very fast. As it is very easy to learn and simple, it would be easy for the client to use, without any complex systems, and also with it's simplicity it will be open for any further developers to improve my software. Another key points about Python is that as it is deeply supported by different communities[^1], it has many different accessible libraries, which makes it really flexible. The flexibilities of possibilities in Python allows us developers to easily find and add different functions in our app. This solution includes functions in different fields such as an App, different screens, databases, and tables. These different functions are all available in Python, therefore I chose to provide a program using Python as a solution.

### KivyMD
First, KivyMD is is free to use[^2]. As well as Python, KivyMD also runs very fast, and it is also flexible. One of the biggest advantages of using KivyMD is that it can be run on a variety of different devices[^3]. It can run on different smartphones sucha as iOS, Android and tablets, and it can run on all major operating systems ((Windows, Linux, macOS))[^3]. As there are a diversity of different audiences using this App (because the audience is ISAK which is a very diverse school), there will be variety of devices that the students use to access this App. Therefore, the flexibity of available devices are very important when designing this App, and that is why I chose KivyMD.

### SQLite
The advantage of using SQLite is that it is very simple and easy to use. SQLite is easy to install and use, and it becomes a single file when saved[^4]. It is also accessible in different devices from home devices (phones) to professional devices (airplanes). SQLite does not need administration, and also does not need a server to run. This means it requires minimal support from the operating system or external library[^5]. As well as KivyMD, this makes SQLite flexible and usable in any device. And in SQLite, a value can be stored in any value in any column, regardless of the data type[^5]. This becomes very important in our App, because we are creating different attributes that the user can input and they are in different values (strings and integers).

[^1]:“Top 10 Reasons Why Python is So Popular With Developers in 2023.” upGrad, 29 September 2022, https://www.upgrad.com/blog/reasons-why-python-popular-with-developers/. Accessed 1 March 2023.
[^2]: Rodriguez, Andres. “kivymd · PyPI.” PyPI, https://pypi.org/project/kivymd/. Accessed 1 March 2023.
[^3]: “Philosophy — Kivy 2.1.0 documentation.” Kivy, https://kivy.org/doc/stable/philosophy.html. Accessed 1 March 2023.
[^4]: “Appropriate Uses For SQLite.” SQLite, 16 December 2022, https://www.sqlite.org/whentouse.html. Accessed 1 March 2023.
[^5]: “What is SQLite? Top SQLite Features You Should Know.” SQLite Tutorial, https://www.sqlitetutorial.net/what-is-sqlite/. Accessed 1 March 2023.

## Success criteria
1. The application will be a well-designed GUI, with availability to access the login screen, sign-up screen, home screen, table screen and an adding screen.
2. The application allows the user to login and logout, or register and the user data will be stored in a database.
3. The user information (password) in the database will be securely stored, encrypted using a hash system. The password will also be longer than 6 letters.
4. The application will allow the user enter all attributes (category, brand, size, color, description, condition) for an item and add an item into the database 
5. The application will allow the user to find a table of items, and remove items from the free store database.
6. The application will allow the user to search for a specific attribute (category, brand, size, color, description, condition), and find an specific item.


# Criteria B: Design

## System Diagram
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/System%20Diagram.png)
**Fig.1**  
This system diagram shows that the program gets an input from the keyboard, then the Mac computer uses existing tools to configurate the inputs to create the output which is the GUI screen.

## Wireframe Diagram
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/wireframe.jpg)
**Fig.2** This diagram, wireframe diagram shows all the screens in the app and which button leads to which screen.

## ER Diagram
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/ER.jpg)
**Fig.3** The ER diagram shows the different tables 'users' and 'items' and it's different properties in the database 'project3db.db'

## UML Diagram
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/UML.jpg)
**Fig.4** 
This is a UML Diagram of the tables and it's attributes.

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/OOP.jpg)
**Fig.5** 
This is a UML diagram of the OOP classes used in the app. It shows the different classes and it's properties.

## Flow diagrams
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/LoginScreen.jpg)
**Fig.6**
Flow diagram for the login screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SignupScreen.jpg)
**Fig.7**
Flow diagram for the Signup screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/HomeScreen.jpg)
**Fig.8**
Flow diagram for the Home screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/Data_Add.jpg)
**Fig.9**
Flow diagram for the Adding data screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/Data_Check.jpg)
**Fig.10**
Flow diagram for the Table screen

## Database Storage 
The data of the different user information and item information will be stored in a SQLite database 'project3db.db'.  
### Users Database
| id | email | password | username |
|-|-|-|-|
| 1 (int. primary key) | apple@apple (str) | pbkdf2_sha256$3000... (str) | apple (str) |
### Items 
| id | category | brand | size | color | description | condition |
|-|-|-|-|-|-|-|
| 1 (int. primary key) | shirt (str) | NIKE (str) | XXS (str) | White (str) | N/A (str) | 8 (int) |

## Test Plan
| Description | Category | Input | Expected Output | Purpose | Success Criteria |
|-|-|-|-|-|-|
| Login Screen - Successful | Unit testing | A username and a password that exists in users | Transition to Home Screen, with thr username on top of the screen | To test if the user can successfully login to their accounts | 1, 2 |
| Login Screen - Failed | Unit testing | A username and a password that doesn't exist in users | An error message that tells that the username or password does not exist | To test the safety of the datas stored in the database | 2 |
| Sign up screen - Successful | Unit testing | A username, email and a passwordx2 with 6 or more letters that doesn't exist in users | Transition to Login Screen, new user data saved into users, with a hashed password | To ensure the safety of the password, and test the adding process of user data into the users database | 1, 2, 3 |
| Sign up screen - Failed | Unit testing | A password with less than 6 letters | Error message saying that the password has to be longer than 6 letters | To test that the user will not be able to set a password with less than 6 letters | 3 |
| Adding data | Unit testing | Different inputs (strings) in the adding screen for values (category, brand, size, color, description) and an integer out put for the value of condition using a slider | The inputs saved into the items table in the database | To test the process of adding items, and have it adding it to the table of items in the database | 4 |
| Data table | Unit testing | None | A screen with a visible table of the table items | To test if the table shows up | 5 |
| Removing items from data table | Unit testing | Pick an item from the table, press the take button | The selected item from items will disappear from the visible and the database table | To test the removing process of an item from the items table | 5 |
| Search items | Unit testing | Specific description of an attribute in the item | The item from items that include the searched word in any of the attribtes will show up | To test process of search bars where when the user searches for a specific word, the item with that attribute will come up | 6 |
| Logging out | Unit testing | Press on 'Logout' in Home Screen | Transition to Login Screen, a pop up checking if the user really wants to log out | To test the transition in screens and the pop up | 1 |
| Transition between screens | Integration testing | Pressing on buttons that are there to change the screen | Transition to another screen | Test to see that the user will be able to swift between different screens | 1 |
| Run the application | System testing | All of the above | All of the above | Test to see that everything in the app is working | 1, 2, 3, 4, 5, 6 |

## Record of Tasks
| Task No | Planned Action | Planned Outcome | Time estimate | Target completion date | Criterion |
|-|-|-|-|-|-|
| 1 | Meet my client | A note of what the problem is and what the client wants | 20min | Feb 10 | A |
| 2 | Write the Problem definition | Completed problem definition | 15min | Feb 11 | A |
| 3 | Write the Design Statement | Completed design statement | 20min | Feb 12 | A |
| 4 | Draw the system diagram | Completed system diagram | 15min | Feb 14 | B |
| 5 | Draw the wirefram diagram | Completed wireframe diagram | 30min | Feb 14 | B |
| 6 | Create a login and sign up system | A system where the client could login to their account or register a new account | 2hours | Feb 16 | C |
| 7 | Creating the code for the login screen | A program that allows the users to either choose to login to the app and move to the Home Screen, or sign up and make a new account | 1hr | Feb 20 | C |
| 8 | Create a database, import it to the project | A database with a table for users and items | 15min | Feb 22 | C |
| 9 | Write a test plan | The table for test plan | 15min | Feb 22 | B |
| 10 | Using the database, create the sign up system | A program that allows the users to input their information and create a new account, inser it into the database | 20min | Feb 24 | C | 
| 11 | Create a password hash system | A program that hashes the password for security when the data information is imported into the database | 30min | Feb 26 | C | 
| 12 | Create a success criteria | Completed success criteria | 20min | Feb 27 | A | 
| 13 | Wrok on my justifications for used tools | Completed Justifications | 1hr | Mar 1 | A | 
| 14 | Wrok on my citations for justifications | Completed citation underneath justification | 5min | Mar 1 | A | 
| 15 | Create a list of existing tools | Completed existing tools | 2min | Mar 1 | C | 
| 16 | Create a home screen | A home screen that allows transition to other screens | 30min | Mar 1 | C | 
| 17 | Create a table 'items' in the database | Table 'items' | 10min | Mar 1 | C | 
| 18 | Create a adding data screen | A screen where the user can input different attributes and will be added into the table | 2hr | Mar 2 | C | 
| 19 | Create a table screen | A screen where the user can check the table 'items', and remove items | 1hr | Mar 2 | C | 
| 20 | Create a search bar 1/2 | A search bar where the user can input a attribute, and that will show up in the table screen | 30min | Mar 2 | C | 
| 21 | Create a search bar 2/2 | A search bar where the user can input a attribute, and that will show up in the table screen | 1hr | Mar 3 | C |
| 22 | Finalize the design of my app | A well-designed app that works | 1hr | Mar 3 | C |
| 23 | Draw the ER diagram | Completed ER diagram | 15min | Mar 3 | B |
| 24 | Draw the UML diagram for database | Completed UML diagram 1/2 | 15min | Mar 4 | B |
| 25 | Draw the UML diagram for OOP | Completed UML diagram 2/2 | 30min | Mar 4 | B |
| 26 | Draw a flow diagram for Login Screen | Completed flow diagram 1/5 | 20min | Mar 5 | B |
| 27 | Draw a flow diagram for Home Screen | Completed flow diagram 2/5 | 20min | Mar 5 | B |
| 28 | Draw a flow diagram for Sign up Screen | Completed flow diagram 3/5 | 40min | Mar 5 | B |
| 29 | Draw a flow diagram for Adding Screen | Completed flow diagram 4/5 | 20min | Mar 5 | B |
| 30 | Draw a flow diagram for Table Screen | Completed flow diagram 5/5 | 20min | Mar 5 | B |
| 31 | Take screen shots of different pages, upload them into github | Screenshots | 10min | Mar 6 | C |
| 32 | Write descriptions for pictures in github | Descriptions | 20min | Mar 7 | B |
| 33 | Write descriptions for python codes | Descriptions | 2hr | Mar 7 | C |
| 34 | Write descriptions for kivy codes | Descriptions | 1hr | Mar 8 | C |


# Criteria C: Development
## Existing tools
OOP paradigm  
KivyMD Library  
Relational databases   
SQLite, ORM  

## Python Code

### Imports
```.py
from kivymd.app import MDApp
from kivymd.uix.datatables import MDDataTable
from kivymd.uix.screen import MDScreen
import sqlite3
import math
from secure_password import encrypt_password, check_password
from kivymd.uix.button import MDFlatButton
from kivymd.uix.dialog import MDDialog
```
This is the items that are imported into the python file. Most of them are from KivyMD, any extra components that I wanted to use. SQLite3 allows the program to connect to the database. Math is used for rounding (used later in sliders), and secure password is another file used for hashing and unhashing, checking the password.

### Database worker
```.py
#database worker
class database_worker:

    def __init__(self, name):
        self.connection = sqlite3.connect(name)
        self.cursor = self.connection.cursor()

    def search(self, query):
        result = self.cursor.execute(query).fetchall()
        return result

    def run_save(self, query):
        self.cursor.execute(query)
        self.connection.commit()

    def close(self):
        self.connection.close()
```
This is the python code that actually connects the database into the python file. Connection and cursor allows us to directly connect to the database, search is used for finding and bringing data from the database, save is for adding and uploading any data into the database, and close is for ending the connection between the python file and the database.

### Home Screen
```.py

#Home Screen
class HomeScreen(MDScreen):

    user_name = None
    dialog = None

    def on_pre_enter(self, *args):
        self.ids.welcome.text = f"Welcome, {self.user_name}"

    def try_add(self):
        print("User trying add data")
        self.parent.current = "Data_Add"

    def try_check(self):
        print("User trying to access data")
        self.parent.current = "Data_Check"

    def try_logout(self):
        if not self.dialog:
            self.dialog = MDDialog(
                title="Confirm logout",
                text="Are you sure you want to logout?",
                buttons=[
                    MDFlatButton(
                        text="CANCEL",
                        theme_text_color="Custom",
                        text_color="#A5D6E5",
                        on_release=self.dialog_close,

                    ),
                    MDFlatButton(
                        text="OK",
                        theme_text_color="Custom",
                        text_color="#A5D6E5",
                        on_release=self.change_screen,


                    ),
                ],
            )
        self.dialog.open()

    def dialog_close(self, *args):
        self.dialog.dismiss(force=True)

    def change_screen(self, *args):
        self.dialog.dismiss(force=True)
        self.parent.current="LoginScreen"

```
This is the code used for the Home Screen. user_name is uploaded from the LoginScreen, which then later when the username is sent,  on_pre_enter will allow the program to show "Welcome, (username)" on the screen. The next 3 functions, add, check and logout are connected to each buttons so when they are pressed, it will move onto a new screen. The logout button is a little bit more complicated than that, as it shows a dialog. The function is saying that if there is no dianog, (that's why there is a 'dialog = None' at the start) MD Dialog will be called. The title, and the text is just text but the title is bigger. The 2 MD FlatButtons are the cancel and the ok buttons, and they both lead to another function which is written below when they are pressed and released. Cancel button leads to the dialog_close function, which basically closes the dialog, and OK will lead to change_screen, which also closes the dialog and changes the current screen back to login screen.

### Adding Screen
```.py
#Adding Screen
class Data_Add(MDScreen):

    def try_submit(self):
        category = self.ids.Category.text
        brand = self.ids.Brand.text
        size = self.ids.Size.text
        color = self.ids.Color.text
        description = self.ids.Description.text
        condition = self.ids.Condition.value
        db = database_worker("project3db.db")
        query = f"Insert into items(category, brand, size, color, description, condition) values('{category}','{brand}','{size}','{color}','{description}','{math.floor(condition)}')"
        db.run_save(query)
        db.close()
        print("Submission")
        self.parent.current = "HomeScreen"

    def try_back(self):
        self.parent.current = "HomeScreen"

```

### Table Screen
```.py
#Table Screen
class Data_Check(MDScreen):

    data_table = None

    def update(self):
        db = database_worker("project3db.db")
        query = "SELECT * FROM items"
        data = db.search(query)
        db.close()
        self.data_table.update_row_data(None, data)

    def try_search(self):
        if self.ids.searchtext.text:
            db = database_worker("project3db.db")
            searchword = self.ids.searchtext.text
            query = f"SELECT * FROM items WHERE category='{searchword}' or brand='{searchword}' or size='{searchword}' or color='{searchword}' or description='{searchword}' or condition='{searchword}'"
            data = db.search(query)
            db.close()
            self.data_table.update_row_data(None, data)
        else:
            self.update()

    def try_remove(self):
        rows_checked = self.data_table.get_row_checks()
        print(rows_checked)
        db = database_worker("project3db.db")
        for r in rows_checked:
            id = r[0]
            query = f"delete from items where id={id}"
            db.run_save(query)
            db.close()
            self.update()

    def on_pre_enter(self, *args):
        self.data_table = MDDataTable(
            size_hint=(.7, .65),
            pos_hint={"center_x": .5, "center_y": .5},
            use_pagination=False,
            check=True,
            column_data=[("id", 40), ("Category", 40), ("Brand", 40), ("Size", 40), ("Color", 40), ("Description", 40), ("Condition", 40)]
        )
        self.data_table.bind(on_row_press=self.row_pressed)
        self.data_table.bind(on_check_press=self.row_pressed)
        self.add_widget(self.data_table)
        self.update()

    def row_pressed(self, table, row):
        pass

    def check_pressed(self, table, current_row):
        pass

    def try_back(self):
        self.parent.current = "HomeScreen"
```

### Login Sreeen
```.py
#Login Screen
class LoginScreen(MDScreen):

    def try_login(self):
        print("User trying to login")
        uname = self.ids.uname.text
        passwd = self.ids.passwd.text
        query = f"select * from users where username = '{uname}' or email = '{uname}'"
        db = database_worker("project3db.db")
        results = db.search(query=query)
        db.close()
        if len(results)==1:
            id, email, hashed, uname = results[0]
            if check_password(user_password=passwd, hashed_password=hashed):
                print("Login successful")
                HomeScreen.user_name=uname
                self.parent.current = "HomeScreen"
            else:
                self.ids.passwd.error = True
                self.ids.uname.error = True
        else:
            self.ids.passwd.error = True
            self.ids.uname.error = True

    def try_register(self):
        print("User trying registration")
        self.parent.current = "SignupScreen"

    def pass_peak(self):
        if self.ids.passwd.password:
            self.ids.passwd.password = False
        else:
            self.ids.passwd.password = True
```

### Signup Screen
```.py
#Sign up Screen
class SignupScreen(MDScreen):

    def try_submit(self):
        uname = self.ids.uname.text
        email = self.ids.email.text
        passwd = self.ids.passwd.text
        passwd_check = self.ids.passwd_check.text

        if passwd != passwd_check:
            self.ids.passwd_check.error = True
        elif len(passwd)<=5:
            self.ids.passwd.error = True
        else:
            hash = encrypt_password(passwd)
            db = database_worker("project3db.db")
            query = f"Insert into users(email, password, username) values('{email}','{hash}','{uname}')"
            db.run_save(query)
            db.close()
            print("Registration complete")
            self.parent.current = "LoginScreen"

    def try_cancel(self):
        self.parent.current = "LoginScreen"
```

### Running the App
```.py
class Project3(MDApp):
    def build(self):
        return

test = Project3()
test.run()
```

## KivyMD Code

### Screen Definitions
```.py
ScreenManager:
    LoginScreen:
        name:"LoginScreen"

    SignupScreen:
        name:"SignupScreen"

    HomeScreen:
        name:"HomeScreen"

    Data_Add:
        name:"Data_Add"

    Data_Check:
        name:"Data_Check"
```

### Login Screen
```.py
<LoginScreen>:
    size:500,500
    FitImage:
        source:"Background.jpg"
    MDCard:
        size_hint:.8,.9
        orientation: "vertical"
        pos_hint: {"center_x":.5,"center_y":.5}
        padding: dp(50) #distance between elements

        MDLabel:
            text:"Login"
            font_style: "H3"
            size_hint:1, .2
            halign:"center"
            pos_hint: {"center_x":.5,"center_y":.5}

        MDTextField:
            id:uname
            hint_text:"Enter your username or email"
            icon_left:"email"

        MDBoxLayout:
            size_hint: 1,.1
            orientation:"horizontal"
            MDTextField:
                id:passwd
                hint_text:"Enter your password"
                icon_left:"key"
                password: True
                size_hint: .7,1
                helper_text_mode: "on_error"
                helper_text: "Username or password is incorrect"
            MDIconButton:
                icon: 'eye'
                pos_hint: {"center_x":1,"center_y":.5}
                on_press:root.pass_peak()

        MDBoxLayout:
            size_hint: 1,.2

            MDRaisedButton:
                id:login
                text:"Login"
                on_press: root.try_login()
                size_hint:.2,.3
                pos_hint: {"center_x":.5,"center_y":.6}
                md_bg_color: "#A5D6E5"

            MDLabel:
                size_hint:.1,.3

            MDRaisedButton:
                id:signup
                text:"Signup"
                on_press: root.try_register()
                size_hint:.2,.3
                pos_hint: {"center_x":.5,"center_y":.6}
                md_bg_color: "#A5D6E5"
```

### Signup Screen
```.py
<SignupScreen>:
    size:500,500
    FitImage:
        source:"Background.jpg"

    MDCard:
        size_hint:.8,.9
        orientation: "vertical"
        pos_hint: {"center_x":.5,"center_y":.5}
        padding: dp(50) #distance between elements

        MDLabel:
            text:"Register"
            font_style: "H3"
            size_hint:1, .1
            halign:"center"
            pos_hint: {"center_x":.5,"center_y":.5}

        MDTextField:
            id:uname
            size_hint: 1,.1
            hint_text:"Enter your username"
            icon_left:"account"

        MDTextField:
            id:email
            size_hint: 1,.1
            hint_text:"Enter your email"
            icon_left:"email"

        MDTextField:
            id:passwd
            size_hint: 1,.1
            hint_text:"Enter your password"
            icon_left:"key"
            password: True

            helper_text_mode: "on_error"
            helper_text: "The password is too short (minimum 6 letters)"

        MDTextField:
            id:passwd_check
            size_hint: 1,.1
            hint_text:"Confirm your password"
            icon_left:"shield-key"
            password: True

            helper_text_mode: "on_error"
            helper_text: "Password does not match"

        MDBoxLayout:
            size_hint: 1,.2

            MDRaisedButton:
                id:submit
                text:"Submit"
                on_press: root.try_submit()
                size_hint:.3,.3
                pos_hint: {"center_x":.5,"center_y":.5}
                md_bg_color: "#A5D6E5"

            MDLabel:
                size_hint:.1,.3

            MDRaisedButton:
                id:cancel
                text:"Cancel"
                on_press: root.try_cancel()
                size_hint:.3,.3
                pos_hint: {"center_x":.5,"center_y":.5}
                md_bg_color: "#A5D6E5"
```

### Home Screen
```.py
<HomeScreen>:
    size:500,500
    FitImage:
        source:"Background.jpg"
    MDCard:
        size_hint:.8,.9
        orientation: "vertical"
        pos_hint: {"center_x":.5,"center_y":.5}
        padding: dp(50) #distance between elements

        MDLabel:
            id:welcome
            text:""
            font_style: "H3"
            size_hint:1, .1
            halign:"center"
            pos_hint: {"center_x":.5,"center_y":.5}

        MDLabel:
            text:"ISAK free store App"
            size_hint:1, .1
            font_size: 65
            halign:"center"
            pos_hint: {"center_x":.5,"center_y":.5}

        MDIconButton:
            icon: 'hanger'
            pos_hint: {"center_x":.5,"center_y":.5}

        MDBoxLayout:
            size_hint: .8,.3
            orientation: "vertical"
            pos_hint: {"center_x":.5,"center_y":.5}

            MDRaisedButton:
                id:add
                text:"Add item"
                on_press: root.try_add()
                size_hint:.7,.6
                md_bg_color: "#A5D6E5"
                pos_hint: {"center_x":.5,"center_y":.5}

            MDLabel:
                size_hint:.2,.1
                pos_hint: {"center_x":.5,"center_y":.5}

            MDRaisedButton:
                id:delete
                text:"Check / Take item"
                on_press: root.try_check()
                size_hint:.7,.6
                md_bg_color: "#A5D6E5"
                pos_hint: {"center_x":.5,"center_y":.5}

            MDLabel:
                size_hint:.2,.1
                pos_hint: {"center_x":.5,"center_y":.5}

            MDRaisedButton:
                id:logout
                text:"Logout"
                on_press: root.try_logout()
                size_hint:.7,.6
                md_bg_color: "#A5D6E5"
                pos_hint: {"center_x":.5,"center_y":.5}
```

### Adding Screen
```.py
<Data_Add>:
    size:500,500
    FitImage:
        source:"Background.jpg"
    MDCard:
        size_hint:.8,.9
        orientation: "vertical"
        pos_hint: {"center_x":.5,"center_y":.5}
        padding: dp(50) #distance between elements

        MDBoxLayout:
            size_hint:1,1
            orientation:"vertical"

            MDLabel:
                text:"Add your item"
                font_style: "H3"
                size_hint:1, .2
                halign:"center"
                pos_hint: {"center_x":.5,"center_y":.5}

            MDTextField:
                id:Category
                hint_text:"Category"
                icon_left:"tshirt-v"

            MDTextField:
                id:Brand
                hint_text:"Brand"
                icon_left:"necklace"

            MDTextField:
                id:Size
                hint_text:"Size"
                icon_left:"move-resize-variant"

            MDTextField:
                id:Color
                hint_text:"Color"
                icon_left:"palette"

            MDTextField:
                id:Description
                hint_text:"Description"
                icon_left:"dots-horizontal"

            MDBoxLayout:
                size_hint:1,.1
                orientation:"horizontal"

                MDLabel:
                    text: "Condition:"
                    color: "#9D9E9E"

                MDLabel:
                    text: "Bad Condition"
                    color: "#9D9E9E"

                MDSlider:
                    id:Condition
                    min: 0
                    max: 10
                    value: 80
                    hint_bg_color: "white"

                MDLabel:
                    text: "Good Condition"
                    color: "#9D9E9E"

            MDLabel:
                text:""
                size_hint:1,.1

            MDBoxLayout:
                size_hint:1,.1
                orientation:"horizontal"

                MDIconButton:
                    id:back
                    on_press: root.try_back()
                    icon: 'arrow-left-bottom'
                    pos_hint: {"center_x":0,"center_y":0}

                MDLabel:
                    text:""
                    size_hint:.8,1

                MDRaisedButton:
                    id:submit
                    text:"Submit"
                    on_press: root.try_submit()
                    pos_hint: {"center_x":1,"center_y":0}
                    md_bg_color: "#A5D6E5"
```

### Table Screen
```.py
<Data_Check>:
    size:500,500
    FitImage:
        source:"Background.jpg"
    MDCard:
        size_hint:.8,.9
        orientation: "vertical"
        pos_hint: {"center_x":.5,"center_y":.5}
        padding: dp(50) #distance between elements

        #search
        MDBoxLayout:
            size_hint:1,.16
            orientation:"horizontal"
            MDTextField:
                id:searchtext
                size_hint: .7,1
                hint_text:"Search for any properties"
                pos_hint: {"center_x":0,"center_y":1}

            MDIconButton:
                id:search
                on_press: root.try_search()
                icon: 'magnify'
                pos_hint: {"center_x":1,"center_y":1}

        MDLabel:
            text:""
            size_hint:1,.8

        MDBoxLayout:
            size_hint:1,.1
            orientation:"horizontal"

            MDIconButton:
                id:back
                on_press: root.try_back()
                icon: 'arrow-left-bottom'
                pos_hint: {"center_x":0,"center_y":0}

            MDLabel:
                text:""
                size_hint:.8,1

            MDRaisedButton:
                id:submit
                text:"Take"
                on_press: root.try_remove()
                size_hint: .1,.7
                pos_hint: {"center_x":1,"center_y":0}
                md_bg_color: "#A5D6E5"
```

## Screen Shots from the app
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Log.png)
**Fig.11**
Login Screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Reg.png)
**Fig.12**
Signup Screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Home.png)
**Fig.13**
Home Screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_pop.png)
**Fig.14**
Pop up for when the user is logging out

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Add.png)
**Fig.15**
Adding items Screen

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Tab.png)
**Fig.16**
Table Screen

# Criteria D: Functionality
## Video
