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

'''

import models
from django.contrib import admin
# Create your models here.
class Order(models.Model):
    order_id = models.IntergerFeild( help_text="Enter  the Order ID")
    customer_name = models.CharFeild(max_length=100,help_text="Enter Customer Name")
    product_name=models.CharFeild(max_length=100, help_text="Entrer the Product Name")
   qty= models.IntegerField(help_text="Enter the Qualtity")
   price=models.FloatFeild(help_text="Entre the Price")

class OrderAdmin(admin.ModelAdmin):
    list_display = ['order_id', 'customer_name', 'product_name', 'qty', 'price']
admin.py
from django.contrib import admin
from .models import Orders,OrderAdmin
# Register your models here.
admin.site.register(Order, OrderAdmin)

'''

## OUTPUT
Include your output


## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
