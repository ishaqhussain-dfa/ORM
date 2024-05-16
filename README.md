# Ex02 Django ORM Web Application
## Date: 
04/04/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![diagram](https://github.com/KGSatheeshKumar/ORM/assets/128453421/cccc114d-5213-4dd6-a103-05b10be93c63)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

```
1) To create Django Project :
  In commandPrompt:
    a) django-admin startproject project1
    b) cd project1
    c) code .

2) To create Application :
    a) Open new terminal
    b) python manage.py startapp app1
3) Models.py :

# Create tables :

from django.db import models

class Student(models.Model):
    stu_id=models.IntegerField()
    stu_name=models.CharField(max_length=30)
    dept=models.CharField(max_length=20)
    email=models.CharField(max_length=30)
    mobile_no=models.IntegerField()

4)Admin.py :

from django.contrib import admin
from app1.models import Student

admin.site.register(Student)

5) Ternimal :

    a) python manage.py makemigration
    b) python manage.py migrate
    c) python manage.py createsuperuser
          - Add UserName and Password for Django server

6) Login to Django administration :
          - Add Student data and Save it


```

## OUTPUT
![s1](https://github.com/KGSatheeshKumar/ORM/assets/128453421/7fbf1487-11be-46f1-8c97-545ad6dde5c9)
![s2](https://github.com/KGSatheeshKumar/ORM/assets/128453421/62e2685e-490a-496e-842f-63658cb0948b)
![s3](https://github.com/KGSatheeshKumar/ORM/assets/128453421/36776863-9f36-4978-9af7-77ced3b821a8)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
