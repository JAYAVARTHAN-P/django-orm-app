# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![omr entity](https://github.com/JAYAVARTHAN-P/django-orm-app/assets/121369281/b44a6f00-8a4d-403f-865b-cea7af5fb921)


## DESIGN STEPS
STEP 1:

Clone the problem from github

STEP 2:

create a new app

STEP 3:

Enter the code for admin.py and model.py

STEP 4:

Execute Django admin and create 10 employees

## PROGRAM
```
admin.py 

from django.contrib import admin
from .models import student,studentAdmin 
admin.site.register(student,studentAdmin)

models.py

from django.db import models
from django.contrib import admin
class student (models.Model):
    sid=models.CharField(max_length=28)
    name=models.CharField(max_length=30)
    regno=models.IntegerField()
    marks=models.IntegerField()
    email=models.EmailField()

class studentAdmin(admin.ModelAdmin):
    list_display=('sid','name','regno','marks','email')
```    



## OUTPUT


![Screenshot (39)](https://github.com/JAYAVARTHAN-P/django-orm-app/assets/121369281/285482be-ffe8-4b8d-bc04-b74af58eeb8f)



## RESULT
The program for coressponding on student database using ORM is executed sucessfully.
