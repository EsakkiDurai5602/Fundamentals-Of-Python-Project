# Fundamentals-Of-Python-Project
This repository contains my submission for the Fundamentals of Python project. The project consists of 15 coding exercises that demonstrate my understanding of basic Python concepts, including data types, control structures, functions, lists, dictionaries, and more.
# Section 1: Python Operators and Control Structures
# Question 1: Calculate the sum of all numbers in a list using a for loop.

numbers = [1, 2, 3, 4, 5]
total = 0
for num in numbers:
    total += num
print(total)  # Output: 15


# Question 2: What is the output of the following code?

x = 5
y = 2
print(x ** y)  # Output: 25


# Question 3: Write a Python program to check if a number is a palindrome using a while loop.

num = 12321
reversed_num = 0
original_num = num
while num != 0:
    remainder = num % 10
    reversed_num = (reversed_num * 10) + remainder
    num = num // 10
if original_num == reversed_num:
    print(True)
else:
    print(False)


# Question 4: What is the output of the following code?

fruits = ['apple', 'banana', 'cherry']
print(fruits[-1])  # Output: cherry


# Question 5: Write a Python program to calculate the average of all numbers in a list using a for loop.

numbers = [1, 2, 3, 4, 5]
total = 0
for num in numbers:
    total += num
average = total / len(numbers)
print(average)  # Output: 3.0


# Section 2: Lists and Dictionaries
# Question 6: Write a Python program to create a dictionary with student names as keys and their grades as values.

students = ['John', 'Alice', 'Bob']
grades = [90, 85, 95]
student_grades = dict(zip(students, grades))
print(student_grades)  # Output: {'John': 90, 'Alice': 85, 'Bob': 95}


# Question 7: What is the output of the following code?

numbers = [1, 2, 3, 4, 5]
print(numbers[1:3])  # Output: [2, 3]


# Question 8: Write a Python program to sort a list of numbers in ascending order using the sorted() function.

numbers = [4, 2, 9, 6, 5]
sorted_numbers = sorted(numbers)
print(sorted_numbers)  # Output: [2, 4, 5, 6, 9]


# Question 9: What is the output of the following code?

fruits = {'apple': 5, 'banana': 10, 'cherry': 15}
print(fruits.get('banana'))  # Output: 10


# Question 10: Write a Python program to create a list of squares of all numbers from 1 to 10 using a list comprehension.

squares = [i ** 2 for i in range(1, 11)]
print(squares)  # Output: [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]


# Section 3: Advanced Topics
# Question 11: Write a Python program to calculate the factorial of a number using recursion.

def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

num = 5
print(factorial(num))  # Output: 120


Question 12: What is the output of the following code?

numbers = [1, 2, 3, 4, 5]
print(list(reversed(numbers)))  # Output: [5, 4, 3, 2, 1]


# Question 13: Write a Python program to create a generator that yields the Fibonacci sequence up to the nth term.

def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        yield a
        a, b = b, a + b

n = 10
fib_sequence = list(fibonacci(n))
print(fib_sequence)  # Output: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]


# Question 14: What is the output of the following code?

import math
print(math.pi)  # Output: 3.14159...

# Question 15: Write a Python program to print the inverted star pyramid of height 5.

def print_inverted_pyramid(height):
    for i in range(height, 0, -1):
        print('* ' * i)

print_inverted_pyramid(5)
