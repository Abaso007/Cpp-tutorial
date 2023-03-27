Conditionals
---
As we have seen in the previous lesson, we can check for multiple conditions using if-else-if statements.
For example, consider the following program, that checks the choice value and outputs the corresponding menu item:
```
int choice = 2;
if(choice == 1) {
  cout << "Coffee";
}
else if(choice == 2) {
   cout << "Tea";
}
else if(choice == 3) {
  cout << "Water";
}
else {
  cout << "Invalid Choice";
}
```


><font color="#AE8E00">When we have a lot of conditions to check, this becomes hard to read and understand. Let's learn how to make it shorter!</font>
---
switch
---
The switch statement can be used to check for equality against a list of values, instead of multiple else if statements.
Here is the previous example using a switch: 
```
switch(choice) {
  case 1:
    cout << "Coffee";
    break;
  case 2:
    cout << "Tea";
    break;
  case 3:
    cout << "Water";
    break;
  default:
    cout << "Invalid Choice";
}
```
Let's understand how it works.

Each case has a value to compare with. When the switch variable's value is equal to a case value, the code inside it is executed, until a break statement is reached.

><font color="#AE8E00">Each case has to have a value and a colon.</font>
---
The break statement is used to terminate the switch, when the case it matched.
If you forget to add the break after each case, the program will continue to execute the code in the next case statements, even if their value does not match the variable's value.
Run this example, to see what happens:
```
switch(choice) {
  case 1:
    cout << "Coffee";
  case 2:
    cout << "Tea";
  case 3:
    cout << "Water";
}
```
><font color="#AE8E00">This type of behavior is called fall-through.</font>
---
default
---
You might notice that there is a default case at the end of the switch statement.
It is used to run code, when none of the cases match:
```
int choice = 8;
switch(choice) {
  case 1:
    cout << "Coffee";
    break;
  case 2:
    cout << "Tea";
    break;
  case 3:
    cout << "Water";
    break;
  default:
    cout << "Invalid Choice";
}
```
><font color="#AE8E00">No break is needed in the default case, as it is always the last statement in the switch.</font>
---
Lesson Takeaways
---
The switch statement is a handy way to check for multiple values.

- Remember, that each case is followed by a value and a colon.
- Each case needs a break statement, or the code of the other cases will continue to get executed. 
- The default case can be used to run code if none of the cases match. 


In the next lesson, we will learn how to combine multiple conditions into one. 


