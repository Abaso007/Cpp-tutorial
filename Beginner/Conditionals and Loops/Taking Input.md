Taking Input
---

Your programs may take user input. For example, these can be commands in a game, or values for an application to process and generate the output.

><font color="#AE8E00">Let's learn how to take input in C++!</font>

---
To take input, use the cin >> command, which is similar to cout in terms of syntax.
Here is an example:
```
int age;
cin >> age;
```
We first declare the variable that will hold our input value.
Then we use it in the cin command.
><font color="#AE8E00">Note that the brackets are different for cin and cout: cin >> and cout <<</font>

---

It's important to use the correct type for the variable when taking input.
For example, let's take a string value as input:
```
string name;
cout << "Please enter your name: "<< endl;
cin >> name;
cout << "You entered:" << name;
```

---
Multiple Inputs
---
You can take multiple inputs throughout your program. 
For example, let's take two integers as input and output their sum:
```
int a, b;
cin >> a;
cin >> b;
cout << a + b;
```

><font color="#AE8E00">Run the code to see how it works. The program will prompt for input and wait till the user provides the required inputs.</font>

---
Similar to cout, you can take multiple inputs on a single line, like this:
```
int a, b;
cin >> a >> b;
```
---
Lesson Takeaways
---
That's how you take input from the user in C++!
First, declare a variable that will store the input. Then, use it in the cin >> command.
The cin >> command is similar to cout <<. It prompts the user for input and stores the entered value in the given variable.
It is important to use the correct type for the variable that will store the input.
In the next lesson, we will learn how to make decisions and check for conditions.