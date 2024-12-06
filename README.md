# Ex02 Django ORM Web Application
# Date:04/12/2024
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

# PROGRAM
```
MODELS.PY:
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
![output02(web)admin](https://github.com/user-attachments/assets/2d716997-c27a-478d-b030-424991950653)
![output02(web)](https://github.com/user-attachments/assets/29f90fa4-9421-4e93-83c3-5f6ab8951b35)
![output02 ii(web)cmd](https://github.com/user-attachments/assets/22e0f01d-22f3-4808-bd63-d2dd3ea5f938)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
