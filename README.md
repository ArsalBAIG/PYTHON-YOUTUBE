1# How to find the average of n numbers in python.

n = int(input("How many numbers to be entered?"))

for i in range(n):
    TotalN = int(input("Enter numbers?"))
    sumN = TotalN
avg = TotalN / n
print("Average will be: ", avg)

2# How to Sum of the First N Positive Integers in Python

#Here the formula's is: n(n + 1)/2
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

numbers = input("Enter some +ive integers? ")
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

colors = ['red', 'green', 'blue', 'black']

print(colors[0], colors[-1])

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

22# How to Get a string which is n copies of a given string in Python

def integer_string(str, n):
    output = ""
    for i in range(n):
        output = output + str
    return output

print(integer_string("Arsal, 3"))

23# How to count the number of items in a list in Python

list_conut = [1, 3, 4, 5, 2, 9]
result = len(list_conut)
print(result)

24# How to find n copies of the first 2 characters of a given string in Python

def first_n(text, n):
    return text[:2] * n

print(first_n("Arsal", 3))

25# How to Check if item is in List in Python
def element_exists(element, list):
    for item in list:
        if item == element:
            return True
        

my_list = [1, 2, 3, 5, 8]
element = 8

if element_exists(element, my_list):
    print("Element exsists. ")
else:
    print("Element doesn't exsists. ")
##Second Method :

fruits = ["apple", "banana", "cherry"]
if "apple" in fruits:
    print("Yes, 'apple' is in the fruits list")

26# How to Create a histogram from a given list of integers in Python

def histogram(items):
    for n in items:
        output = " "
        times = n
        while(times > 0):
            output += "*"
        # Here, time is decrementing.
            times -= 1
        print(output)

histogram([1, 2, 3, 4, 5])

27# How to Turn a list into a string in Python

def convert_list(list):
    output = ""
    for item in list:
        output += str(item)
    return output

print(convert_list([1, 2, 3 , 4]))

28# How to print even numbers in the given range in Python

start = int(input("Enter the lower range? "))
end = int(input("Enter the upper range? "))

if start % 2 != 0:
    start += 1

for i in range(start, end + 1, 2):
    print(i)

29# How to compare lists in Python

l1 = [10, 20, 30, 40, 50]
l2 = [20, 30, 50, 40, 70]
l3 = [50, 10, 30, 20, 40]

l1.sort()
l2.sort()
l3.sort()

if l1 == l2:
    print("List 1 is as same as list 2. ")
else:
    print("List 1 is'nt same as list 2. ")
if l1 == l3:
    print("List 1 is as same as list 3. ")
else:
    print("List 1 is'nt same as list 3. ")

30# How to Find the Greatest Common Divisor GCD in Python

import math
a = 45
b = 55

result = math.gcd(a, b)
# Here, GDC means greatest common division which is actually the table on which the values are divisible.
print(f"The GDC of {a} and {b} is: {result}")

31# How to Find least common multiple LCM in Python

from math import lcm
result = lcm(2, 4, 7)
print("The LCM is: ", result)

32# How to sum of three given integers in python

def threeNum(x, y, z):
    return x + y + z

num1 = 9
num2 = 4
num3 = 8

print(threeNum(num1, num2, num3))

33# How to Add two objects if both objects are an integer type in Python

class Integer:
    def __init__(self, value):
        self.value = value
    
    def __add__(self, other):
        #Here, we check that is 'other' a instance of Integer class or not if not then we raise an Error.
        if not isinstance(other, Integer):
            raise TypeError("Both values must be integer type! ")
            #Here, value is attribute.
        return Integer(self.value + other.value)

num1 = Integer(23)
num2 = Integer(33)
result = num1 + num2
#Here, we print sum of two objects using result.value
print("Sum of two objects will be: ", result.value)
                                                ::Another example::

class Number:
    def __init__(self, first):
        self.first = first
    
    def __sub__(self, second):
        if not isinstance(second, Number) or second < 0:
            raise TypeError("Both values must be +ive. ")
            #Here, first is an attribute of second.
        return Number(self.first - second.first)
    
num1 = Number(23)
num2 = Number(33)
result = num2 - num1
print(f"The Subtarction will be: {result.first}")

34# How to Display name, age, address in three different lines in Python

def details():
    name, age = "Arsal", 19
    address = "Civil lines, Jhang Sadar."
    print("Name is:{}\n Age: {}\n Address: {}".format(name, age, address))

details()

35# How to solve {x + y } * {x + y} in Python

x = 3
y = 8
result = x * x + y * y + 2 * x * y
print(f"(x + y)^ 2 = {result}")

36#  How to compute the future value of rate of interest and a number of years in Python

amount = 7000
interest_rate = 3.5
time = 9
# Here, the formula is: P(1 + r/ 100)^ t.

future_amount = amount * ((1 + (interest_rate / 100)) ** time)
print(round(future_amount))

37# How to calculate the distance between two points in Python

x1, y1 = 5, 8
x2, y2 = 9, 1

distance = ((x1 - x2)**2 + (y1 - y2)**2)**0.5
print(f"Distance b/w {x1} and {x2} and {y1} and {y2} is= {distance:.2f}")

37# Caculate the size of python? 

import struct
print(struct.calcsize("P") * 8)

38# How to Check the OS name, platform and release information in Python

import platform
import os

print(os.name)
print(platform.system())
print(platform.release())

39# How to get path and name of a file that is currently executing in Python

import os
print("Current File is: ", os.path.realpath(__file__))

40# How to Sort Counter by value in Python

from collections import Counter
#Here, ({'a': 5}) is a object.
y = Counter({'a': 5, 'b' : 3, 'c' : 8})
#Here, ({'a': 5}) we assign values to each key in a dict.
sorted_y = sorted(y, key= y.get, reverse= True)

for key in sorted_y:
    print(key)

41# How to convert height in feet and inches to centimeters in python

feet = int(input("Enter your height(feet)"))
inches = int(input("Enter your height(inches)"))
#feet & inches to inches
inches += feet * 12
#height in cm
cm = round(inches * 2.54, 1)
print(f"Your height is: {cm}cm")

42# How to Calculate the hypotenuse of a right angled triangle in python

import math
pre = 9.0
base = 8.3
x  = math.hypot(pre, base)
print(round(x,2))

43# How to convert the distance in feet to inches, yards, and miles in python

dis_feet = int(input("Enter distance in feet: "))
dis_inches = dis_feet * 12
dis_yards = dis_feet / 3.0
dis_miles = dis_feet / 5280.0

print(f"Distance in inches is: {dis_inches} inches")
print(f"Distance in inches is: {dis_yards:.2f} yards")
print(f"Distance in inches is: {dis_miles:.2f} miles")

44# How to calculate body mass index in Python

weight_kg = int(input("Enter weight in kg's "))
height_cm = float(input("Enter height in cm's"))
height_m = height_cm / 100

BMI = weight_kg / (height_m ** 2)
print("Your BMI is: ", round(BMI, 2))

45# How to Convert seconds to day, hour, minutes and seconds in Python

import datetime
second = 60
#Here, we use timedelta to rep diff b/w time which is second in this case.
time = datetime.timedelta(seconds= second)
#Here, we convert time into string to rep days, hours, min.
formated_time = str(time)
print(formated_time)

46# How to Find ASCII Value of Character in Python

def get_ASCII(char):
    return ord(char)

character = 'B'
print("ASCII value of char is: ", get_ASCII(character))

47# How to Extract extension from filename In Python

file_name = 'mymodule.txt'
#Here, (".") means it finds the . first and then adds 1 and then prints upto the end
extension = file_name[file_name.index(".") + 1:]
print(f"File Extension: {extension}")

48# How to Get Current Date & Time in Python

from time import gmtime, strftime
#Here, gmtime is a function that holds values like %H, %M etc
formated_time = strftime("%H:%M %Y-%M-%S")
print(formated_time)

49# How to Check if a String is a Number in Python    

def is_num(string):
    return string.isdigit()

input_string = '7865'
if is_num(input_string):
    print("it's a number")
else:
    print("it's not! ")

50# How to Swap two variables in Python

x = 9
y = 0

temporary = x
x = y
y = temporary
print("X = ", x)
print("Y = ", y)

51# How to Join or Concatenate N strings in Python

string = ["Hello", "World!"]
delimeters = " "
output = delimeters.join(string)
print(output)

52# How to Find file path or directory in Python

import os
path = os.path.dirname(os.path.realpath(__file__))
print("Directory path is: ", path)

53# How to Multiply all numbers in the list in Python

def multiplyList(myList):
    output = 1
    for x in myList:
        output *= x
    return output

list1 = [1, 3, 5]
list2 = [2, 4, 6]

print(multiplyList(list1))
print(multiplyList(list2))

54# How to get current module object in Python

from inspect import getmodule
from math import sqrt
#Here, we use sqrt to demonstrate the exact location where sqrt is stored. We can also use some other function instead of sqrt it's just an example.
print(getmodule(sqrt))

55# How to Add leading zeroes to a string in Python
1- 
my_string = '908'
print(my_string.zfill(6))

2-
#Here, 1 indicates integer 1 and '04' indicated that we insert 0 on the left and insert until it's width is 4.
formated_output = format(1, '04')
print(formated_output)

56# How to Convert pressure in kilopascals to pounds in Python

kilopascals = float(input("Enter the pressure in kilopascal's? "))
psi = round(kilopascals * 0.1450, 3)
millimeterHg = round(kilopascals * 7.500, 3)
atm = round(kilopascals * 0.0098756, 3)

print(f"Pressure in psi is {psi} or Pressure in millimeter of Hg {millimeterHg} or Pressure in atm is {atm}")

57# How to get the copyright information in Python

import sys
print(sys.copyright)
print()

58# How to Get the size of an object in bytes in Python

import sys
x = 9
size = sys.getsizeof(x)
print(size)

59# How to Get the identity of an object in Python

x = 89
print(id(x))

60# How to Retrieve file properties In Python

from pathlib import Path
file_path = Path("/PYTHON LEARNING/mymodule.txt")
file_info = file_path.stat()

print("File size: ", file_info.st_size)
print("Last modified Time is: ", file_info.st_mtime)

61# How to print positive numbers in a list in Python

listing = [3, -8, 5, -3, -7]
for num in listing:
    if num > 0:
        print(num, end= " ")

62# How to Sum all values of a counter in Python

from collections import Counter
myCount = Counter([3, 4, 3, 6, 9 ])
#Here, values() is used to show no of values in Counter.
total_count = sum(myCount.values())
print("Total Count is: ", total_count)

63# How to Calculate the time runs of a program in Python

import time
start_time = time.time()
for i in range(1000):
    pass

end_time = time.time()

execution_time = end_time - start_time
print(f"Execution Time: {execution_time:.5f}")

64# How to validate IP address in Python

import ipaddress

def valid_ip(ip):
    try:
        ip_obj = ipaddress.ip_address(ip)
        print(f"{ip} is a valid IP Address. (version{ip_obj.version})")
    except ValueError:
        print(f"{ip} is invalid IP Address. ")

valid_ip("192.168.0.1")

65# How to Find the number of characters in a file using Python

def count_char(filename):
    with open(filename, "r") as file:
        text = file.read()
        chars = len(text)

    print(f"No of char in {filename} : {chars}")

count_char("mymodule.txt")

66# How to Insert a string in the middle of a string in Python

def insert_middle_string(org_string, insert_string):
    middle = len(org_string) // 2
#Here, printing org_string upto middle value and then insert_string and then printing remaning middle of org_string to end.
    return f"{org_string[:middle]} {insert_string}{org_string[middle:]}"
new_string = insert_middle_string("Cast","Baig")
print(new_string)

67# How to Remove a newline in Python

original_string = "Hello, world!\n"
cleaned_string = original_string.replace("\n", "")
print(cleaned_string)

68# How to Reverse a string in Python
1-
org_string = 'Hello there!'
reverse = org_string[::-1]
print(reverse)

2-
org_string = 'Hello there!'
reverse_list = list(reversed(org_string))
#Here, "" indicates spaces and join is use for concatenation.
reverse_string = "".join(reverse_list)
print(reverse_string)

69# 
