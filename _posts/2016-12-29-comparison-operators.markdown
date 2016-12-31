---
layout: default
title:  "Comparison Operators"
date:   2016-12-28 5:15:00
categories: Python-Tutorial
---

# Comparison Operators
In this lecture we will be learning about Comparison Operators in Python. These operators will allow us to compare variables and output a Boolean value (True or False).

If you have any sort of background in Math, these operators should be very straight forward.

First we'll present a table of the comparison operators and then work through some examples:

# Table of Comparison Operators

| Operator | Description | Example |
| --- | --- | --- |
| ==	|If the values of two operands are equal, then the condition becomes true. |	(a == b) is not true. |
| !=	| If values of two operands are not equal, then condition becomes true.	| (a != b) is true |
| <>	| If values of two operands are not equal, then condition becomes true.	|(a <> b) is true. This is similar to != operator. |
| >	| If the value of left operand is greater than the value of right operand, then condition becomes true.	| (a > b) is not true. |
| <	| If the value of left operand is less than the value of right operand, then condition becomes true.	| (a < b) is true. |
| >=	| If the value of left operand is greater than or equal to the value of right operand, then condition becomes true. |	(a >= b) is not true. |
| <=	| If the value of left operand is less than or equal to the value of right operand, then condition becomes true.	| (a <= b) is true. |

Let's now work through quick examples of each of these.

## Equal

```python
In [3]: 2 == 2
```
```python
Out[3]: True
```
```python
In [4]: 1 == 0
```
```python
Out[4]: False
Not Equal
```
```python
In [5]: 2 != 1
```
```python
Out[5]: True
```
```python
In [6]: 2 != 2
```
```python
Out[6]: False
```
```python
In [7]: 2 <> 1
```
```python
Out[7]: True
```
```python
In [8]: 2 <> 2
```
```python
Out[8]: False
Greater Than
```
```python
In [9]: 2 > 1
```
```python
Out[9]:True
```
```python
In [10]:2 > 4
```
```python
Out[10]:False
Less Than
```
```python
In [11]:2 < 4
```
```python
Out[11]:True
```
```python
In [12]:2 < 1
```
```python
Out[12]:False
Greater Than or Equal to
```
```python
In [13]:2 >= 2
```
```python
Out[13]:True
```
```python
In [14]:2 >= 1
```
```python
Out[14]:True
Less than or Equal to
```
```python
In [15]:2 <= 2
```
```python
Out[15]:True
```
```python
In [16]:2 <= 4
```
```python
Out[16]:True
```

 Great! Go over each comparison operator to make sure you understand what each one is saying. But hopefully this was straightforward for you

## Next we will cover [chained comparison operators](python-tutorial/2016/12/29/chained-comparison-operators.html)