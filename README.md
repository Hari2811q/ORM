# Ex02 Django ORM Web Application
## Date: 29/12/2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

```
admin.py
from django.contrib import admin
from .models import Football_Player,Football_PlayerAdmin 
admin.site.register(Football_Player,Football_PlayerAdmin)

models.py
from django.db import models
from django.contrib import admin 
class Football_Player(models.Model):
    Player_id=models .CharField(max_length=15)
    Player_name=models.CharField(max_length=30)
    Event=models.CharField(max_length=50)
    Category=models.CharField(max_length=20)
    Age=models.IntegerField()
class Football_PlayerAdmin(admin.ModelAdmin):
    list_display=["Player_id","Player_name","Event","Category","Age"]    


```

##OUTPUT


![2023-10-18](https://github.com/Akshayasakthivels/ORM/assets/144870561/68a8d137-e1a3-44de-8d67-d78f12940cb2)
