Functions
---
A function is a block of code designed to perform a particular task.
For example, your program can have functions like login(), logout(), convert(), withdraw(), etc.

> The purpose of a function is to create it once and call it multiple times when needed to perform particular tasks.
---
You can define your own functions to perform your desired tasks. 
Here is an example:
```
void hello() {
  cout << "Hello!" << endl;
  cout << "I am a sample function";
}
```
The code above declares a function called "hello", which outputs 2 lines of text.
> Note that the name of the function is followed by parentheses ().
The statements of the function are inside curly braces {}.
---
Let's understand how the function is defined:
```
void hello() {
  cout << "Hello!" << endl;
  cout << "I am a sample function";
}
```
void means that this function does not have a return value. You will learn more about return values later in this module.
hello is the name of the function.

---

Now that we have our function defined, we can use it in our program by "calling" it.
To call a function, type its name followed by a set of parentheses. 
For example, let's call our hello function in main:
```
int main() {
  hello();
}
```
> Run the code to see the result.
---
Calling a Function
---
You can call a function as many times as necessary. 
```
#include <iostream>
using namespace std;

void hello() {
  cout << "Hello!" << endl;
  cout << "I am a sample function" << endl;
}

int main() {
  hello();
  hello();
  hello();
}
```
Also, note that it is important to declare the function prior to calling it.
If we put the declaration of our function after main, we would get an error.

---
Lesson Takeaways
---

Awesome! Remember the following points:

 - Functions are reusable; we define them once and can call them multiple times.
 - To call a function, use its name, followed by parentheses. 
 - The void keyword means that the function does not return a value. 


We will learn about return values in the next lessons, so stay tuned!