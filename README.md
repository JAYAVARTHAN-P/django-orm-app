# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

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
![ex2](https://github.com/JAYAVARTHAN-P/django-orm-app/assets/121369281/f36b362c-9bfd-41b8-a9ce-97b140f14c04)


## RESULT
The program for coressponding on student database using ORM is executed sucessfully.
