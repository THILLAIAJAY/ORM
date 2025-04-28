# Ex02 Django ORM Web Application
## Date: 24-04-2025
## Developed By: Thillaiajay L 

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/59e29248-b510-4bbc-9cd1-6b6fa664f3db)

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
## admin.py


from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

## models.py


from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20, help_text="Employee")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid', 'name','salary', 'age', 'email')
```

## OUTPUT

Include the screenshot of your admin page.

![Screenshot 2025-04-24 092224](https://github.com/user-attachments/assets/e1fa13b1-be8e-42da-bfa1-0f09856af2dc)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
