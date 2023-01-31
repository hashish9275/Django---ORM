# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![img](newmapdiagram.jpg)

## DESIGN STEPS

### STEP 1:
Create a newapp using django-admin and upload python code

### STEP 2:
Create a meaningful table containing students details in ORM

### STEP 3:
Push the code to github

## PROGRAM

```
admin.py:

from django.contrib import admin
from .models import Studentdetail,StudentdetailAdmin


admin.site.register(Studentdetail,StudentdetailAdmin)
# Register your models here.


models.py:

from django.db import models
from django.contrib import  admin


#Create your models here.
#Create your models here.
# Create your models here.
class Studentdetail(models.Model):
    referencenumber = models.CharField(max_length=10, primary_key=True , help_text="your reference no ")
    name= models.CharField(max_length=100)
    department = models.CharField(max_length=200)
    age=models.IntegerField()
    email=models.EmailField()
class StudentdetailAdmin(admin.ModelAdmin):
    list_display = ('referencenumber', 'name', 'department', 'age', 'email')
```

## OUTPUT

![img](outputss.jpg)


## RESULT
Thus the experiment was executed successfully.
