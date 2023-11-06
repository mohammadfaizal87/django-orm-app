# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![ER](https://github.com/mohammadfaizal87/django-orm-app/assets/147139206/14ff3c0c-5626-400e-b5b1-06e7a1a36e13)

## DESIGN STEPS

### STEP 1:
create a table using required detailsb in Django_ORM

### STEP 2:
upload the python code

### STEP 3:

push the code to github

## PROGRAM
#FROM Admin.py
from django.contrib import admin
from .models import Student,StudentAdmin
# Register your models here.
admin.site.register(Student,StudentAdmin)

#FROM Models.py
from django.db import models
from django.contrib import admin

# Create your models here.
class Student (models.Model):
    referenceno=models.CharField(primary_key=True,max_length=20,help_text="referenceno")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    mobileno=models.IntegerField()
class StudentAdmin (admin.ModelAdmin):
    list_display=('referenceno','name','age','email','mobileno')

## OUTPUT
![Screenshot 2023-11-06 060809](https://github.com/mohammadfaizal87/django-orm-app/assets/147139206/65da73ae-f97e-4586-b496-c9a03838c30b)


## RESULT
The Program is Executed Successfully.
