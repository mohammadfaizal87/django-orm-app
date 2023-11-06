# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
create a table using required detailsb in Django_ORM

### STEP 2:
upload the python code

### STEP 3:

push the code to github

## PROGRAM
admin.py
from django.contrib import admin from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)

models.py
from django.db import models from django.contrib import admin

class Student (models.Model): referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number") name=models.CharField(max_length=100) age=models.IntegerField() email=models.EmailField() mobilenumber=models.IntegerField() class StudentAdmin(admin.ModelAdmin): list_display=('referencenumber','name','age','email','mobilenumber')

## OUTPUT

## RESULT
The Program is Executed Successfully.
