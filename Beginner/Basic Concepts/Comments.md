Comments
---
One more thing before we complete the first module.

Comments are annotations in the code that explain what the code is doing.
Code is for computers, while comments are for humans who read and work with the code.

---
A single-line comment starts with two forward slashes and continues until it reaches the end of the line. 

For example:
```
// storing the height of the user
double height = 74.8; // this is just a demo value
```
><font color="#AE8E00">Adding comments as you write code is a good practice, because they provide clarification and understanding when you need to refer back to it, as well as for others who might need to read it.</font>

---
You can also comment out lines of code, in case they are work-in-progress or you don't want to delete them yet:
```
double height = 74.8;
//int weight = 40;

cout << height;
//cout << weight;   
```

><font color="#AE8E00">The commented lines of code will get ignored when you run the program.</font>

---
Multi-Line Comments
---
If you need to comment out multiple lines, or write a multi-line comment, you can use the /* */ symbols, like this:
```
/*  This is just a
  demo program
  that outputs a name */

string name  = "James";
```
Anything between the /* and */ symbols becomes a comment.


><font color="#AE8E00">You can also use multi-line comments to comment out multiple lines of code.</font>

---
Lesson Takeaways
---
Now you know how to add comments to your code!
Here are some key takeaways:
Comments are explanatory statements that explain what the code is doing.
They can contain notes, todos as well as code that is work-in-progress.
- // starts a single line comment.
- /* */ is used for multi-line comments.