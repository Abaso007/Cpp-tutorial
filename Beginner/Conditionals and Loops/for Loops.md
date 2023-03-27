for Loops
---
The for loop has the following form:
```
for(int i=1;i<=5;i++) {
  cout << i << endl;
}
```
This will output the numbers 1 to 5.

---
Let's look at the code again and understand how it works:
```
for(int i=1;i<=5;i++) {
  cout << i << endl;
}
```
The for loop has 3 components in the parentheses:
- The first part runs once when we enter the loop and initializes the variable.
- The second part is the condition of the loop.
- The third part runs every time the loop runs.

><font color="#AE8E00">Note the semicolons between the components.</font>
---
You can have any type of condition and any type of increment statements in the for loop.
```
for(int i=3;i<=20;i+=2) {
  cout << i << endl;
}
```
><font color="#AE8E00">The for loop is best when we know the number of times we need to run the loop.</font>
---
Remember the break; statement that was used in switch to stop it when a case was matched?
It can also be used to stop a loop. 
```
for(int i=0;i<10;i++) {
  if(i==5) {
    break;
   }
  cout << i << endl;
}
```
The loop will stop when i reaches the value 5.
><font color="#AE8E00">Run the code to see the result.</font>
---
continue
---
The continue statement skips the current loop iteration and continues with the next one.

```
for(int i=0;i<10;i++) {
  if(i==5) {
    continue;
  }
  cout << i << endl;
}
```
><font color="#AE8E00">This will skip the number 5. Run the code to see the result.</font>
---
Lesson Takeaways 
---
Great progress! Here is a summary:
- The for loop has the following syntax:
```
for(init; condition; increment) {
   //code
}
```
 - The break statement can be used to stop a loop.
-  The continue statement can be used to skip the current iteration of the loop and jump to the next one. 