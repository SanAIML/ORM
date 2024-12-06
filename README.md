# Ex02 Django ORM Web Application
# Date:21/10/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).


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
models.py

from django.db import models
from django.contrib import admin
class loan (models.Model):
    Loan_Id=models.CharField(max_length=20,primary_key=True)
    Name=models.CharField(max_length=100)
    Age=models.IntegerField()
    Salary=models.IntegerField()
    Loan_applied_date=models.DateField()
    Loan_amount=models.IntegerField()
    Email=models.EmailField()
    Phone_no=models.IntegerField()


class loanAdmin(admin.ModelAdmin):
    list_display=('Loan_Id','Name','Age','Salary','Loan_applied_date','Loan_amount','Email','Phone_no')


admin.py
from django.contrib import admin
from .models import loan,loanAdmin
admin.site.register(loan,loanAdmin)




```
# OUTPUT
![alt text](<Screenshot 2024-11-29 104015.png>)

![Screenshot 2024-12-06 141553](https://github.com/user-attachments/assets/58f5a1f4-3944-444d-923e-04c8fe5024ad)

# ER DIAGRAM
![BANK LOAN](https://github.com/user-attachments/assets/f9f2ee6b-4c21-4db8-a0af-bc262ff865b3)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
