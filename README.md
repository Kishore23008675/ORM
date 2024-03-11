# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot 2024-03-11 201712 (1)](https://github.com/Kishore23008675/ORM/assets/144979375/7579f896-8583-4536-a58b-eef248d5b698)

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
admin.py 

from django.contrib import admin
from .models import book_details,book_detailsAdmin
admin.site.register(book_details,book_detailsAdmin)

model.py

from django.db import models
from django.contrib import admin
class book_details(models.Model):
    no=models.IntegerField(primary_key=True);
    name=models.CharField(max_length=66);
    author=models.CharField(max_length=66);
    year=models.IntegerField();
    price=models.IntegerField();

class book_detailsAdmin(admin.ModelAdmin):
    list_diaplay=("no","name","author","year","price");
```
```
from django.db import models
from django.contrib import admin


# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    number=models.IntegerField()

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','number')
```
## OUTPUT

Include the screenshot of your admin page.
![Screenshot 2024-03-11 201332](https://github.com/Kishore23008675/ORM/assets/144979375/85c0097e-fae6-4e2c-843f-29350ae7ae5e)
![Screenshot 2024-03-11 201355](https://github.com/Kishore23008675/ORM/assets/144979375/cf6d8d8d-3b38-4bee-94a6-25c839189696)
## RESULT
Thus the program for creating a database using ORM hass been executed successfully
