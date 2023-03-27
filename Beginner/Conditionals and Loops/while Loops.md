Loops
---

A loop allows you to repeat a block of code multiple times.
><font color="#AE8E00">For example, a game can use a loop to take input from the user controls, or a warehouse management system can loop through all items in the warehouse and perform calculations.</font>
---
while Loop
---
The while loop takes a condition and repeats its statements while the condition is true.
For example: 
```
int num = 5;
while(num > 0) {
  cout << num << endl;
  num = num - 1;
}
```
The while loop checks for the condition num > 0. If it evaluates to true, it executes the statements within its body. Then it checks for the statement again and repeats.
><font color="#AE8E00">The given code will output the numbers 5 to 1 and then stop, as num will reach 0.</font>
---
Let's have a look at the code again:
```
int num = 5;
while(num > 0) {
  cout << num << endl;
  num = num - 1;
}
```
The statement num = num - 1 decreases the value of num by 1 each time the loop runs. 
This is important, as without it the loop would run forever.

---
Increment & Decrement
---
As it's common to increment and decrement a variable's value by 1 in loops, C++ provides special increment and decrement operators.
For example, num=num-1 can be shortened to num--:
```
int num = 5;
while(num > 0) {
  cout << num << endl;
  num--;
}
```
---
Increment
---
Similarly, num++ will increase the value of num by 1:
```
int num = 1;
while(num <= 10) {
  cout << num << endl;
  num++;
}
```
---
Shorthand Operators
---
Sometimes you might need to increase or decrease the value of a variable by a different value than 1. 
For these cases, C++ provides shorthand operators, too!
For example, x=x+2 can be shortened to x+=2:
```
int num = 0;
while(num <= 10) {
  cout << num << endl;
  num+=2;
}
```
This will output only the even numbers from 0 to 10.
><font color="#AE8E00">Similarly, there are shorthand operators for other mathematical operations, such as -= for subtraction, *= for multiplication, etc.</font>
---
do while
---
Another variation of the while loop is do-while.
Here is an example:
```
int num = 0;
do {
  cout << num << endl;
  num+=2;
} while(num <= 10);
```
The difference with a while loop is that the condition is checked after the code, meaning the code in the do is executed at least once, even if the condition is false.
Also, note the semicolon after the while condition.
><font color="#AE8E00">Try changing the condition in the code above to something false and see the result.</font>
---
Lesson Takeaways
---
Great progress! Here is a summary about the while loop:

- The code in the while loop runs as long as the condition is true.
- The ++ and -- operators are used to increase and decrease the value of a variable by one.
- C++ provides shorthand operators to perform mathematical operations on a variable, for example num=num * 5 can be written as num * = 5.
- The do-while loop is similar to a while loop, but it is guaranteed to run at least once. 


We will learn about another loop type in the next lesson and perform calculations with it! 