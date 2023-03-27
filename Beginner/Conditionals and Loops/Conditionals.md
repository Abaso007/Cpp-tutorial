Decision Making
---
Conditional statements are used to perform different actions based on different conditions. 
For example, a banking application can set different rates based on the client types, a ticketing application can apply discounts based on the age of the buyers, etc. 

Let's learn how to create such programs.

---
The if statement allows you to run a specified code if a given condition is true.
Here is the syntax:
```
if(condition) {
  //code to run
}
```
><font color="#AE8E00">Note that the code of the if statement is enclosed in curly brackets { }.</font>
---
if Statement
---
The following comparison operators may be used to form the condition:

"<" less than
">" greater than
"!=" not equal to
"==" equal to
"<=" less than or equal to
">=" greater than or equal to
For example: 

```
int points = 89;
if(points >= 70) {
  cout << "Success!";
}
```
><font color="#AE8E00">The message will be output only if the condition is satisfied.</font>
---
Remember that you need to use two equal signs (==) to test for equality, since a single equal sign is the assignment operator.
For example, let's check the day value for equality:
```
if(day == 7) {
  cout << "Sunday";
}
```
---
else Statement
---
You can use the else statement after an if statement, if you want to run a code in case the condition is false.
For example:
```
int grade = 52;
if(grade >= 75) {
  cout << "Passed!";
}
else {
  cout << "Failed";
}
```
The grade value is less than 75, so the code in the else statement will run.

><font color="#AE8E00">In all previous examples only one statement was used inside the if/else statement, but you may include as many statements as you want.</font>

---
Nested if Statements
---
You can use one if-else statement inside another if or else statement.
For example:
```
int age = 24;
if(age >= 65) {
  cout << "Senior";
}
else {
  if(age >= 18) {
    cout << "Adult";
  }
  else {
    cout << "Child";
  }
}
```

><font color="#AE8E00">You can nest as many if-else statements as you want, however the code will become harder to read and understand.</font>

---
Nested if-else statements become hard to read and maintain. This is why C++ provides the else if statement.
Here is our previous example, written using else if statements:
```
if(age >= 65) {
  cout << "Senior";
}
else if(age >= 18) {
  cout << "Adult";
}
else {
  cout << "Child";
}
```
><font color="#AE8E00">You can include as many else if statements as you need.
Lesson Takeaways</font>
---
Decision making is easy, right?
You can check for a condition using the if statement.
In case the condition is false, the code in an else statement can be executed.
Here is a generic structure of if-else statements:
```
if(condition) {
  //some code
} 
else if(condition) {
//some other code
} 
else {
  //some other code
}
```
We will learn about another decision making statement in the next lesson.