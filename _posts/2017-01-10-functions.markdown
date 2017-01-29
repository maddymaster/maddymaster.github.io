---
layout: default
title:  "Functions"
date:   2017-01-10 17:50:00
categories: Python-Tutorial
---

## Functions
### Introduction to Functions
This lecture will consist of explaining what a function is in Python and how to create one. Functions will be one of our main building blocks when we construct larger and larger amounts of code to solve problems.

So what is a function?

Formally, a function is a useful device that groups together a set of statements so they can be run more than once. They can also let us specify parameters that can serve as inputs to the functions.

On a more fundamental level, functions allow us to not have to repeatedly write the same code again and again. If you remember back to the lessons on strings and lists, remember that we used a function len() to get the length of a string. Since checking the length of a sequence is a common task you would want to write a function that can do this repeatedly at command.

Functions will be one of most basic levels of reusing code in Python, and it will also allow us to start thinking of program design (we will dive much deeper into the ideas of design when we learn about Object Oriented Programming).

### def Statements
Let's see how to build out a function's syntax in Python. It has the following form:

```python
In [3]:
def name_of_function(arg1,arg2):
    '''
    This is where the function's Document String (doc-string) goes
    '''
    # Do stuff here
    #return desired result
```

We begin with def then a space followed by the name of the function. Try to keep names relevant, for example len() is a good name for a length() function. Also be careful with names, you wouldn't want to call a function the same name as a built-in function in Python (such as len).

Next come a pair of parenthesis with a number of arguments separated by a comma. These arguments are the inputs for your function. You'll be able to use these inputs in your function and reference them. After this you put a colon.

Now here is the important step, you must indent to begin the code inside your function correctly. Python makes use of whitespace to organize code. Lots of other programing languages do not do this, so keep that in mind.

Next you'll see the doc-string, this is where you write a basic description of the function. Using iPython and iPython Notebooks, you'll be ab;e to read these doc-strings by pressing Shift+Tab after a function name. Doc strings are not necessary for simple functions, but its good practice to put them in so you or other people can easily understand the code you write.

After all this you begin writing the code you wish to execute.

The best way to learn functions is by going through examples. So let's try to go through examples that relate back to the various objects and data structures we learned about before.

### Example 1: A simple print 'hello' function
```python
In [4]:
def say_hello():
    print 'hello'
Call the function
```
```python
In [5]:
say_hello()
hello
```
### Example 2: A simple greeting function
Let's write a function that greets people with their name.

```
In [6]:
def greeting(name):
    print 'Hello %s' %name
```
```python
In [7]:greeting('Jose')
```
```python 
Hello Jose
```
Using return
Let's see some example that use a return statement. return allows a function to return a result that can then be stored as a variable, or used in whatever manner a user wants.

### Example 3: Addition function
```python
In [8]:def add_num(num1,num2):
    return num1+num2
```
```python
In [9]:add_num(4,5)
```
```python
Out[9]:9
```
```python
In [10]:# Can also save as variable due to return
result = add_num(4,5)
```
```python
In [11]:print result
9
```
What happens if we input two strings?

```python
In [12]:print add_num('one','two')
onetwo
```
Note that because we don't declare variable types in Python, this function could be used to add numbers or sequences together! We'll later learn about adding in checks to make sure a user puts in the correct arguments into a function.

Lets also start using break,continue, and pass statements in our code. We introduced these during the while lecture.

Finally lets go over a full example of creating a function to check if a number is prime ( a common interview exercise).

We know a number is prime if that number is only evenly divisible by 1 and itself. Let's write our first version of the function to check all the numbers from 1 to N and perform modulo checks.
```python
In [8]:def is_prime(num):
    '''
    Naive method of checking for primes. 
    '''
    for n in range(2,num):
        if num % n == 0:
            print 'not prime'
            break
    else: # If never mod zero, then prime
        print 'prime'
```
```python        
In [9]:is_prime(16)
not prime
```
Note how we break the code after the print statement! We can actually improve this by only checking to the square root of the target number, also we can disregard all even numbers after checking for 2. We'll also switch to returning a boolean value to get an example of using return statements:

```python
In [15]:import math

def is_prime(num):
    '''
    Better method of checking for primes. 
    '''
    if num % 2 == 0 and num > 2: 
        return False
    for i in range(3, int(math.sqrt(num)) + 1, 2):
        if num % i == 0:
            return False
    return True
```
```python
In [16]:is_prime(14)
```
```python
Out[16]:False
```
Great! You should now have a basic understanding of creating your own functions to save yourself from repeatedly writing code!