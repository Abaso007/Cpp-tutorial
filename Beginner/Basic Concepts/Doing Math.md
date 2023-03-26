Doing Math
---
C++ supports a number of arithmetic operators that can be used to perform calculations.
Let's declare two variables and output their sum:
```
int a = 8;
int b = 24;
std::cout << a+b;
```
---
The result of a calculation can be assigned to another variable.
For example, let's use subtraction to demonstrate:
```
int price = 20;
int discount = 5;
int total = price - discount;
```
---
Multiplication
---

Multiplication is done using the * operator.
For example:
```
int points = 28;
int level = 3;
int result = points * level;
```
---
Division
---
Division is done using the / operator.
Let's calculate how many days there are in 500 hours:
```
int hours = 500;
int days = hours / 24;
```
><font color="#AE8E00">The result will be a whole number, as we are dividing two integers.</font>

---
In case we need a more precise result, which includes decimal points, we can use doubles:
```
double hours = 500;
double days = hours / 24;
```

><font color="#AE8E00">Run the code to see the result.</font>
---
Remainder
---
The % remainder operator (also called the modulo) is used to find the remainder of a division.
Let's find how many days will be left over if we divide 500 days into weeks:
```
int days = 500;
int result = days % 7;
```

---
Lesson Takeaways
---
Doing math is easy and fun! Here are some key takeaways:

You can use basic math operators to perform calculations with values and variables.

- "+" is addition
- "-" is subtraction
- "/" is division
- Dividing integers results in an integer.
- % finds the remainder of a division.
  
We'll learn more about variables in the next lesson!