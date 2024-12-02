# Ex02 Django ORM Web Application
# Date: 30/10/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books
```
# PROGRAM
MODEL.PY:

from django.db import models
from django.contrib import admin
class Bank(models.Model):
  

    bank_name=models.CharField(max_length=100)
    branch_name=models.CharField(max_length=100) 

    customer_name=models.CharField(max_length=100)
    account_no=models.IntegerField()
    mobile_no=models.IntegerField()
    Email=models.EmailField()

class BankAdmin(admin.ModelAdmin):
    	list_display= ('bank_name', 'branch_name', 'customer_name', 'account_no', 'mobile_no', 'Email')


ADMIN.PY:

from django.contrib import admin

from .models import Bank,BankAdmin
admin.site.register(Bank,BankAdmin)
```
# OUTPUT
Include the screenshot of your admin page.
![output02(web)](https://github.com/user-attachments/assets/ba8acc69-082b-477c-905f-0dea64876631)

![output02 i(web)cmd](https://github.com/user-attachments/assets/f795d417-b991-48e1-8b9e-7d908f4b3e73)
![output02 ii(web)cmd](https://github.com/user-attachments/assets/ec93657e-b513-460c-a602-440220024b24)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
