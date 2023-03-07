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
One of the reason I chose Python is because it is one of the fastest-growing languages in the world, as it is considered as one of the best programming languages for machine learning[1]. Python runs very fast. As it is very easy to learn and simple, it would be easy for the client to use, without any complex systems, and also with it's simplicity it will be open for any further developers to improve my software. Another key points about Python is that as it is deeply supported by different communities[1], it has many different accessible libraries, which makes it really flexible. The flexibilities of possibilities in Python allows us developers to easily find and add different functions in our app. This solution includes functions in different fields such as an App, different screens, databases, and tables. These different functions are all available in Python, therefore I chose to provide a program using Python as a solution.

### KivyMD
First, KivyMD is is free to use[2]. As well as Python, KivyMD also runs very fast, and it is also flexible. One of the biggest advantages of using KivyMD is that it can be run on a variety of different devices[3]. It can run on different smartphones sucha as iOS, Android and tablets, and it can run on all major operating systems ((Windows, Linux, macOS))[3]. As there are a diversity of different audiences using this App (because the audience is ISAK which is a very diverse school), there will be variety of devices that the students use to access this App. Therefore, the flexibity of available devices are very important when designing this App, and that is why I chose KivyMD.

### SQLite
The advantage of using SQLite is that it is very simple and easy to use. SQLite is easy to install and use, and it becomes a single file when saved[4]. It is also accessible in different devices from home devices (phones) to professional devices (airplanes). SQLite does not need administration, and also does not need a server to run. This means it requires minimal support from the operating system or external library[5]. As well as KivyMD, this makes SQLite flexible and usable in any device. And in SQLite, a value can be stored in any value in any column, regardless of the data type[5]. This becomes very important in our App, because we are creating different attributes that the user can input and they are in different values (strings and integers).

**Citations**  
1. “Top 10 Reasons Why Python is So Popular With Developers in 2023.” upGrad, 29 September 2022, https://www.upgrad.com/blog/reasons-why-python-popular-with-developers/. Accessed 1 March 2023.
2. Rodriguez, Andres. “kivymd · PyPI.” PyPI, https://pypi.org/project/kivymd/. Accessed 1 March 2023.
3. “Philosophy — Kivy 2.1.0 documentation.” Kivy, https://kivy.org/doc/stable/philosophy.html. Accessed 1 March 2023.
4. “Appropriate Uses For SQLite.” SQLite, 16 December 2022, https://www.sqlite.org/whentouse.html. Accessed 1 March 2023.
5. “What is SQLite? Top SQLite Features You Should Know.” SQLite Tutorial, https://www.sqlitetutorial.net/what-is-sqlite/. Accessed 1 March 2023.

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

## Wireframe Diagram
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/wireframe.jpg)
**Fig.2** 

## ER Diagram
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/ER.jpg)
**Fig.3** 

## UML Diagram
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/UML.jpg)
**Fig.4** 

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/OOP.jpg)
**Fig.5** 

## Flow diagrams
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/LoginScreen.jpg)
**Fig.6**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SignupScreen.jpg)
**Fig.7**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/HomeScreen.jpg)
**Fig.8**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/Data_Add.jpg)
**Fig.9**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/Data_Check.jpg)
**Fig.10**

## Database Storage 
The data of the different user information and item information will be stored in a SQLite database 'project3db.db'.  



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



# Criteria C: Development
## Existing tools
OOP paradigm
KivyMD Library
Relational databases
SQLite, ORM

## Python Code
## KivyMD Code

## Screen Shots
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Log.png)
**Fig.11**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Reg.png)
**Fig.12**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Home.png)
**Fig.13**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_pop.png)
**Fig.14**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Add.png)
**Fig.15**

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Project/Pics/SS_Tab.png)
**Fig.16**
