# Ex01 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 5 Car 

## PROGRAM
Include your program
```

from django.db import models
from django.contrib import admin
class studentdb(models.Model):
    student_name = models.CharField(max_length=25)
    student_id = models.IntegerField()
    student_email = models.EmailField()
    join_date = models.DateField()

class studentdbAdmin(admin.ModelAdmin):
    list_display = ('student_name','student_id','student_email','join_date')


from django.contrib import admin
from.models import studentdb, studentdbAdmin
admin.site.register(studentdb, studentdbAdmin)

```


## OUTPUT
Include your output
![59689547525 jpj](https://github.com/user-attachments/assets/b520ab11-99b7-4c1c-893e-2bed9d6b16dd)



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
