# Ex02 Django ORM Web Application
## Date: 08/09/2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
<img width="1920" height="1080" alt="Movie" src="https://github.com/user-attachments/assets/a6973e5d-66fe-4b56-bc27-c2424681df4e" />



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
from django.db import models
from django.contrib import admin
class Movies(models.Model):
    M_ID = models.IntegerField(primary_key=True)
    M_name = models.CharField(max_length=100)
    Release_date=models.DateField()
    Director=models. CharField(max_length=50)
    Actors=models. CharField(max_length=100)
 
class MoviesAdmin(admin.ModelAdmin):
    list_display=(M_ID', ‘M_name', ‘Release_date’, 
                                  ‘Director', Actors ')
```
```
from django.contrib import admin
from .models import Movies, MoviesAdmin
admin.site.register(Movies, MoviesAdmin)
```

## OUTPUT


<img width="1920" height="1200" alt="Screenshot (1)" src="https://github.com/user-attachments/assets/b2ff3103-8404-4c0e-a6a0-2f535d64edbd" />

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
