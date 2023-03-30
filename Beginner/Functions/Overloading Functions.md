Overloading Functions
---
Let's have a look at one of our example functions:
```
void sum(int x, int y) {
  cout << x+y << endl; 
}
```
The function takes two integers as its parameters and outputs their sum.
What if we want the function to also work for other data types, such as doubles? 
Let's learn how to make that work.

---
C++ allows you to define a function with the same name but different parameter data types.
Here is our sum function, using double parameters:
```
void sum(double x, double y) {
  cout << x+y << endl;
}
```
We used the same function name, and changed the parameter data types.
This is called function overloading.

---
Now, when we call the function, the correct version will be called based on the type of the argument.
Here is an example:
```
sum(42, 31);
sum(3.14, 5.66);
```
The function that corresponds to the given parameters will be called.

---
You cannot overload function declarations that differ only by return type.
The following declaration results in an error:
```
int demo(int x) {
  return x;
}
double demo(int x) {
    return x/2;
}
```

---
Default Arguments
---
Another handy thing when working with functions are default arguments.
When defining a function, you can specify a default value for each of the last parameters.
If the corresponding argument is missing when you call a function, it uses the provided default value.
```
int area(int x, int y=1) {
  return x*y;
}
```
As you can see, we can simply assign a value to the parameter in the parentheses.
Now we can call the function with or without that parameter: 
```
cout << area(8, 5) << endl;
cout << area(6) << endl;
```
> The default value will be used for the parameter, when no value is provided.
---
Lesson Takeaways
---
You did it! This was the last lesson of the course!

- Overloading functions allows you to use the same name of the function with different parameter data types.
- Default arguments allow to specify a default value for the last parameters of the function by assigning them values right in the definition.

---
