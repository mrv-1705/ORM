# Ex02 Django ORM Web Application
## Date: 5/04/24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-04-05 212526](https://github.com/mrv-1705/ORM/assets/114565075/92a5b0c3-4f76-4c6c-bd9a-3ba3f2750632)


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

Admins.py
```
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```
Models.py
```
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text='Employee ID')
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
## OUTPUT


![Screenshot 2024-04-05 210510](https://github.com/mrv-1705/ORM/assets/114565075/4ce6c574-0bcf-4e97-b7c9-85a965deedad)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
