1# How to find the average of n numbers in python.

n = int(input("How many numbers to be entered?"))

for i in range(n):
    TotalN = int(input("Enter numbers?"))
    sumN = TotalN
avg = TotalN / n
print("Average will be: ", avg)

2# How to Sum of the First N Positive Integers in Python

x = int(input("Enter Total no of values? "))
sum_for = (x * (x + 1)) // 2
print("Sum will be: ", sum_for)

3# How to get time in python program.

from datetime import datetime 
now = datetime.now()
formated_time = now.strftime("%H:%M")
print(formated_time)

4# How to access environment variables in Python

import os
print(os.environ)

5# How to find which python version are you using now.

import sys
print(sys.version_info)

6# How to find the Area of Circle in python.

from math import pi
def circleArea(r):
    return pi * (r ** 2)
radius = float(input("Enter the radius of circle? "))
print(f"The radius of circle will be: {circleArea(radius):.2f}")

7# How to print first and last name in python?

firstN = input("Enter your first name? ").capitalize()
lastN = input("Enter your last name? ").capitalize()
print(f"Hello {firstN} {lastN}")

8# How to create a list and tuple with comma separated numbers in Python
