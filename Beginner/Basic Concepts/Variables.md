Variables
---
Every program works with values.
A variable lets you store a value by assigning it to a name. The name can be used to refer to the value later in the program. 

><font color="#AE8E00">For example, in game development, you would use a variable to store how many points the player has scored.</font>

---
Every variable has a type, which defines the type of the value it holds. 
A variable can hold a text value, a number, a decimal, etc.
We are already familiar with text values - they are created using quotes:
```
"this is some text"
```
><font color="#AE8E00">A text value is called a String. </font>

---
Let's create a variable of type string:
```
string message;
```
This creates a variable called message of type string.
Now, our variable message can hold string values.
><font color="#AE8E00">In programming terms, the process of creating a variable is called declaration.</font>

---
After declaring our variable, we can assign it a value using the assignment = operator:
```
string message;
message = "Welcome";
```
Now, message holds the value "Welcome". 
><font color="#AE8E00">Note, that the string value should be in quotes.</font>

---
Now, after declaring and assigning a value, we can output the value of our variable:
```
string message;
message = "Welcome";
cout << message;
```

---
We can combine the declaration and assignment into one statement, like this:
```
string message = "Welcome";
```

><font color="#AE8E00">This is handy when we already know the value for our variable and makes the code shorter and more readable.</font>

---
A variable can change its value during the program multiple times. 
For example, the message can change based on the language:
```
string message = "Welcome";
message = "Bienvenue";
```
---
Lesson Takeaways
---
Awesome! Here are some key takeaways:
- A variable has a name and a type of the value it holds. 
- To declare a variable use the type followed by the name of the variable.
- You can assign a value to the declared variable using the = operator.
- A variable can change its value during the program, by being assigned to a new value.

We will learn about more variable types in the next lesson! 
