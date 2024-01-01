# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
clone the problem from github
### STEP 2:
create a new app in django project
### STEP 3:
Enter the code for admin.py and models.py
Write your own steps

## PROGRAM
models.py
from django.db import models
from django.contrib import admin
# Create your models here.
class Student (models.Model):
referencenumber=models.CharField(max_length=20,help_text="reference
number")
name=models.CharField(max_length=100)
age=models.IntegerField()
email=models.EmailField()
mobileno=models.IntegerField()
class StudentAdmin(admin.ModelAdmin):
list_display=
('referencenumber','name','age','email','mobileno')
admin.py
from django.contrib import admin
from .models import Student, StudentAdmin
admin.site.register(Student,StudentAdmin
class Student (models.Model):
referencenumber=models.CharField(max_length=20,help_text="reference 
number")
 name=models.CharField(max_length=100)
 age=models.IntegerField()
 email=models.EmailField()
 mobileno=models.IntegerField()
class StudentAdmin(admin.ModelAdmin):
 list_display=
('referencenumber','name','age','email','mobileno')
 admin.py
 from django.contrib import admin
from .models import Student, StudentAdmin
# Register your models here.
admin.site.register(Student,StudentAdmin)
## OUTPUT

![image](https://github.com/HARIPRIYASIVAKUMAR/django-orm-app/assets/147477684/ea547edd-bf17-4006-a05d-54e8e41338cd)



## RESULT
The program for creating a database using ORM has been executed sucessfully.
