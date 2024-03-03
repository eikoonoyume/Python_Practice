# Exercise 1 from pythonpractice.org
Create a program that asks the user to enter their name and their age. Print out a message addressed to them that tells them the year that they will turn 100 years old. Note: for this exercise, the expectation is that you explicitly write out the year (and therefore be out of date the next year). If you want to do this in a generic way, see exercise 39.

Extras:

Add on to the previous program by asking the user for another number and printing out that many copies of the previous message. (Hint: order of operations exists in Python)
Print out that many copies of the previous message on separate lines. (Hint: the string "\n is the same as pressing the ENTER button)

name = input("Please enter your name: ")
age = int(input("Please enter your age: "))
century_year = int(2024) + (int(100) - age)
print(name + ", you will turn 100 years old in the year " + str(century_year))

message = (name + ", you will turn 100 years old in the year " + str(century_year))
message_copy = int(input("Please enter a number for number of copies: "))
print(message_copy * str(message +".\n"))

# Site Solution:
name = input("What is your name: ")
age = int(input("How old are you: "))
year = 2024 - age + 100
print(name + ", you will be 100 years old in the year " + str(year))

# Update each year
import datetime
import time

name = input("Please enter your name: ")
age = int(input("Please enter your age: "))
currentYear = datetime.date.today().year
century_year = int(currentYear) + (int(100) - age)
phrase(name + ", you will turn 100 years old in the year " + str(century_year))
print(phrase)

message = phrase
message_copy = int(input("Please enter a number for number of copies: "))
print(message_copy * str(message +".\n"))
