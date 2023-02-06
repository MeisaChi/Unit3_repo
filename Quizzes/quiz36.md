## Code
```.py
class Person:
    def __init__(self, name:str, age:int):
        self.name = name
        self.age = age

    def get_name(self)->str:
        return self.name.title()

    def get_age(self)->int:
        return self.age

class Student(Person):
    def __init__(self, name:str, age:int, grade:int):
        super().__init__(name=name, age=age)
        self.grade = grade

    def get_grade(self)->int:
        return self.grade

sam = Student(name="sam", age=12, grade=6)
print(f"{sam.get_name()} is {sam.get_age()} years old, and is in grade {sam.get_grade()}.")

class Classroom:
    def __init__(self):
        self.students_list = []

    def add_student(self, student)->str:
        self.students_list.append(student)

asama25 = Classroom()
sam2 = asama25.add_student(sam)
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz36.png)
