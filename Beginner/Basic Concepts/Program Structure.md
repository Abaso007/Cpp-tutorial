C++ Program
---
Let's look at the code of the whole program and learn about all the code statements and what they do.

Here is the code to output text:
```
#include <iostream>

int main() {
  std::cout << "C++ is awesome";
}
```
---
The first line of the code adds the <iostream> header to the program:
```
#include <iostream>
```
A header is a file that contains functions and commands. 
The <iostream> header in C++ contains the cout command, that we used for outputting text. This is why we need to include it in our program, to enable us to use the cout command.

><font color="#AE8E00">The #include command is used to add a header file to the program. Note the # symbol, it's necessary!</font>

---
Let's take a look at our whole program:
```
#include <iostream>

int main() {
  std::cout << "C++ is awesome";
}
Click to run
```
After the header, you see the following code:
```
int main() 
{ 
    //something
}
```
Each C++ program has a entry point, or starting point, which is a function called main.

><font color="#AE8E00">We will cover each keyword of the definition in later lessons, when learning about functions. For now, remember that the main function needs to be declared identical to the code above.</font>

---
Curly brackets { } indicate the beginning and end of a function, which can also be called the function's body. The code inside the brackets indicates what the function does when executed.
```
int main() {
  cout << "C++ is awesome";
}
```
When we run the code, the cout command will be executed.

---
The main function can contain multiple lines of code.
For example, let's try to output two different text values:
```
cout << "This is the first line";
cout << "This is the second line";
```


><font color="#AE8E00">When you run this code, you'll notice that the output is on the same line. This is happening because the cout command does not add a new line at the end of the output.</font>

---
To add a new line, you can use the endl command, like this:

```
cout << "This is the first line" << endl;
cout << "This is the second line";
```
This adds a new line after the first text. You can use as many endl commands as you need.

><font color="#AE8E00">Note, that you can use the << symbols to separate different outputs in a single cout statement. For example: cout << "One" << endl << "Two" << endl;</font>

---
Lesson Takeaways
---
Great job! Now you know how to create valid C++ programs.

Remember the following important points:

- The #include statement is used to add a header file to the program.
- The using command is used to tell the program which namespace to use.
- To use the cout command, you need to include the <iostream> header
- The starting point of C++ programs is the function called main, which includes the code that you want to run.
- The endl command is used to add a new line to the output.

---