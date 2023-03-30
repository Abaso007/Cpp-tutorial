Function Parameters
---
Functions can have parameters, which they can use in their code.
The parameters are defined in the parentheses, and can be used like variables in the function.
For example, let's add a string name parameter to our hello function:
```
void hello(string name) {
  cout << "Hello, " << name << endl;
}
```
The function above takes a string called name as its parameter, which is used in the function's output.

---
Now, when calling the function, we need to pass it a value for the name parameter inside the parentheses:

```
void hello(string name) {
  cout << "Hello, " << name << endl;
}

int main() {
  hello("James");
  hello("Amy");
}
```
This way, we can call our function with different parameters and generate different results based on them.

> The values passed as parameters when calling the function are called arguments.
---
Multiple Parameters
---
Functions can take multiple parameters. For that, we simply need to separate them using commas, for example:
```
void sum(int x, int y) {
  cout << x+y << endl;
}
```
Now, our sum() function takes two integer parameters.

> Note, that we need to define the data type and name for each parameter.
---
Now, when calling the function, we need to provide all the parameters:
```
void sum(int x, int y) {
  cout << x+y << endl;
}

int main() {
  sum(21, 56);
}
```
Note that the arguments need to match the parameters and must be passed in the same order, separated by commas.

---
Function parameters allow you to use the same function for different values, making it reusable.
For example, we can take user input and pass it as a function argument:
```
void square(int x) {
  cout << x*x << endl;
}

int main() {
  int a;
  cin >> a;
  square(a);
}
```
> Run the code to see how it works.
---
Lesson Takeaways
---
Function parameters are really helpful and allow you to use the same function for different values!

Here is a summary:

 - You can define parameters in the parentheses, by providing the data type and a name. 
 - Multiple parameters need to be separated by commas.
 The parameters are available in the function as variables of the given names.
 - When calling a function, you need to provide its parameters in the same order, as defined, separated by commas. 


You will learn how to return values in the next lesson. 