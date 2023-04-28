# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![er](/images/er.png)

## DESIGN STEPS

### STEP 1:
Fork and clone the repositary in to your IDE.
### STEP 2:
Create a django project and an app and a superuser account and run the server.
### STEP 3:
Modify changes in settings and write ur code on models and admin and run the server.
### STEP 4:
Login in to admin using your superuser account and populate the records.

## PROGRAM
```python
from django.db import models
from django.contrib import admin


# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    phone_no=models.IntegerField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','phone_no')
```

## OUTPUT

![op](/images/op.png)

### Server output

![sop](/images/sop.png)


## RESULT
Thus we developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
