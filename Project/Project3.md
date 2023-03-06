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

### Justification

**Python (PyCharm)**

**KivyMD**

**SQLite**

**Citations**


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
| 3 | Write the Design Statement | Completed design statement | 20mins | Feb 12 | A |
| 4 | Draw the system diagram | Completed system diagram | 15mins | Feb 14 | B |
| 5 | Draw the wirefram diagram | Completed wireframe diagram | 30mins | Feb 14 | B |
| 6 | Create a database for login and sign up | A system where the client could login to their account or register a new account | 2hours | Feb 16 | C |
| 7 | Creating the code for the login screen | A program that allows the users to either choose to login to the app and move to the Home Screen, or sign up and make a new account | 1hr | Feb 20 | C |
| 8 | Create a database, import it to the project | A database with a table for users and items | 15mins | Feb 22 | C |
| 9 | Write a test plan | The table for test plan | 15min | Feb 22 | B |
| 10 | Using the database, create the sign up system | A program that allows the users to input their information and create a new account, inser it into the database | 20min | Feb 24 | C | 
| 11 | Create a password hash system | A program that hashes the password for security when the data information is imported into the database | 30min | Feb 26 | C | 
| 12 | Create a success criteria | Completed success criteria | 20min | Feb 27 | A | 

| 13 | Write the list of techniques used     |make people being able to know what techniques we used| 10min         | Dec 13                 | C | 
| 14 | Write the Computational thinking part     |make people being able to know what kind of computational thinking we used| 45min         | Dec 13                 | C | 
| 15       | Write the prptotype codes    |make people being able to know what we coded| 40min         | Dec 13                 | C | 
| 16       | Make a poster which explains what we did in the project    |make client being able to know the situation of temperature and humidity in Isak| 120min         | Dec 13                 | C | 
| 17       | Make a video which explains the contents what we did for this project    |make people being able to know the work that we have been working on| 120min         | Dec 13                 | C | 


# Criteria C: Development
## Existing tools
OOP paradigm
KivyMD Library
Relational databases
SQLite, ORM

## Python Code
## KivyMD Code
