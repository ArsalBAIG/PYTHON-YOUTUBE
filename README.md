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

numbers = int(input("Enter some +ive integers? "))
list = numbers.split(",")
#Here, tuple is used to convert list into tuple.
tuple = tuple(list)

print("List is: ", list)
print("Tuple is: ", tuple)

9# How to extract extension from filename in python

import os
file_name = "mymodule.txt"
#Here, [1] is used to get .txt and file_name is used to get mymodule
file_extention = os.path.splitext(file_name)[1]

print(file_extention)

10# Display the first and last colors from a given list in Python
(Do it yourself).

11# Display a sample examination schedule in Python

exam_starting = (27, 6, 2024)
print(f"The exam will start from {exam_starting[0]} / {exam_starting[1]} / {exam_starting[2]}")

12# How to Read a number n and compute n+nn+nnn in python

n = input("Enter any single no? ")
# Here, we convert 'n' into string due to concatination.
temprary = str(n)
x1 = temprary + temprary
x2 = temprary + temprary + temprary
Addition = int(n) + int(x1) + int(x2)
print("Sum will be: ", Addition)

13# How to print a calendar for the given month and year in Python

import calendar
year = int(input("Enter the year?" ))
month = int(input("Enter the month? "))

if 1 <= month <= 12:
    calculate = calendar.month(year, month)
    print(f"The calender of year {year} and month {month}")
    print(calculate)
else:
    print("Please enter b/w 1 to 12 months. ")

14# How to Calculate number of days between two dates in Python

from datetime import datetime
birthDate = datetime.strptime("15/12/2004", "%d/%m/%Y")
currentDate = datetime.strptime("7/6/2024", "%d/%m/%Y")
diff = currentDate - birthDate
print(f"No of days you live are {diff.days}")

15# How to find Volume and Surface Area of Sphere in Python

PI = 3.13
r = float(input("Enter the value of radius? "))
volume = 4 * PI * r * r
print(f"Vol will be: {volume:.2f} cm^3")

16# How to find the difference between two numbers in Python

def subtract(num):
    if num < 15:
        return num - 5
    else:
        return (num * 3) / 4
    
print(subtract(12))
17# Calculate sum of three numbers if the values are equal then return thrice of their sum in Python

def thrice(x, y, z):
    Total = x + y + z

    if x == y == z:
        Total *= 3
    return Total

print(thrice(2, 2, 2))

18# How to Get a new string from a given string in Python

# We use slicing for this purpose.
string = "Hello my name is Arsal!"
newString = string[3: 8]
print(newString)

19# How to reverse a number using slice operations in python

user_input = int(input("Enter any +ive integer? "))
reverse = int(str(user_input)[::-1])
print(reverse)

20# How to find the Biggest and Smallest of 3 numbers using lists in Python

def find_large_small(number):
    largest = max(number)
    smallest = min(number)
    return largest, smallest

num_list = [12, 45, 2, 41, 31, 10, 8, 6, 4]
# Here, we unpack largest_num, smallest_num into two seperate variables.
largest_num, smallest_num = find_large_small(num_list)
print(f"Largest no is: {largest_num}")
print(f"Smallest no is: {smallest_num}")

21# How to find area of a triangle in Python

def area_of_triangle(base, height):
    return (base * height) / 2

print(f"Area of Tri is: {area_of_triangle(5, 9):.2f}")

