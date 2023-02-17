# Quiz 44

Questions:

1. How many tables are there in the database?

![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz44/question1.png)

2. How many Male inhabitants are Friendly?
```.py
select count(*) from Inhabitant where gender = 'Male' and state = 'Friendly';
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz44/question2.png)

3. What is the average gold by village?
```.py
select avg(gold) from INHABITANT group by villageid;
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz44/question3.png)

4. How many items are there that start with the letter “A”
```.py
select count(*) from item where item like 'a%';
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz44/question4.png)

5. How many different jobs are there? 
```.py
select job, count(*) from inhabitant group by job;
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz44/question5.png)

6. What are the items owned by the herbalists?
```.py
select personid from inhabitant where job = 'Herbalist';
select * from item where owner = 4 or owner = 18
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz44/question6.png)
