# Ex02 Django ORM Web Application
## Date: 25/03/2025

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![er diagram (1)](https://github.com/user-attachments/assets/646463bb-400b-48fc-a97d-3391cb4055c0)



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
'''
models.py
from django.db import models
from django.contrib import admin
class Loan(models.Model):
   loan_id=models.IntegerField(primary_key=True)
   loan_type=models.CharField(max_length=30)
   loan_amount=models.FloatField()
   cust_acntno=models.IntegerField()
   cust_name=models.CharField(max_length=50)

class LoanAdmin(admin.ModelAdmin):
    list_display=('loan_id','loan_type','loan_amount','cust_acntno','cust_name')

admin.py
from django.contrib import admin


from.models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)



## OUTPUT

![Screenshot 2024-11-23 143310](https://github.com/user-attachments/assets/990d6156-7731-452d-88db-d41f14f547ff)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
