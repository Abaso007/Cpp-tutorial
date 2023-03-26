Types
---
C++ supports many different types for your variables, based on their value.
The int type is used to store whole numbers (called integers in programming):
```
int points = 128;
```
---
Decimals
---
To store decimals (or floating point numbers), C++ provides the float and double data types.

For example: 
```
double temp = 84.2;
```
><font color="#AE8E00">The term "floating point" refers to the fact that a varying number of digits can appear before and after the decimal point. You could say that the decimal has the ability to " float".</font>
---

The float type is also used to store decimals. 
To specify that the value is a float, we need to use the letter f after it:
```
float length = 5.31f;
```
This tells C++ to use the value as a float, instead of double.

---
float vs double
---
By default, decimal values are of type double float uses less storage in the memory, but is not as precise as the double type. This means that calculations that use floats are faster than the ones that use double, however, the results are less accurate in terms of the decimal digits.

><font color="#AE8E00">The best practice is to use double, if you do not have any specific requirements to use float.</font>
---
Char
---
The char type is used to store a single character.
It is similar to declaring a string, but uses single quotes for the value:
```
char x = 'H';
```

---
Boolean
---
The bool type can only hold values: either true or false.
It is used when working with conditions.
For example: 
```
bool online = false;
```
The online variable can show if the user is online or not.

><font color="#AE8E00">When you run the code, you'll notice that the output is 0, instead of false. This is because the boolean value true corresponds to 1, while the value false corresponds to 0.</font>
---
Lesson Takeaways
---
Great job! Here are some key takeaways about data types:

- int is used to hold whole numbers (integers)
- double stores decimals.
- float is similar to double, but has less precision and requires less memory. You need to prefix the value with the letter 'f' to create floats.
- char holds a single character.
- bool can have one of the following values: true or false. 

We will learn how to use variables and make calculations in the next lesson.