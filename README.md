# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![ER](https://github.com/mohammadfaizal87/django-orm-app/assets/147139206/14ff3c0c-5626-400e-b5b1-06e7a1a36e13)

## DESIGN STEPS

### STEP 1:
clone the repository here inside the folder ex02
### STEP 2:
After cloning the folder with the repository name django-orm-appwill be created.
### STEP 3:
Now move into the django-orm-appfolder then move into the folder myproj where manage.py file is located.
### STEP 4:
Now give the commands python3 manage.py startapp myapp to create myapp. Then change the necessary settings in the settings.py. 
### STEP 5:
Then enter the codes in models.py andd admin.py then give the commands:
python3 manage.py makemigrations
python3 manage.py migrate
### STEP 6:
Now  run the program using the command: python manage.py 
runserver 0:8000

## PROGRAM
```py

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
```

## OUTPUT
![Screenshot 2023-11-06 060809](https://github.com/mohammadfaizal87/django-orm-app/assets/147139206/65da73ae-f97e-4586-b496-c9a03838c30b)


## RESULT
The Program is Executed Successfully.
