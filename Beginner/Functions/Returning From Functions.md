Return Values
---
The functions we have seen so far output their result.
In some cases we do not need to output the result, but need to assign it to a variable to work with it in our program.
In these cases, we need our function to return the result value, instead of outputting it. 

---

The Return Type
---
Let's have a look at a function from our previous examples:
```
void sum(int x, int y) {
  cout << x+y << endl;
}
```
It takes two parameters and outputs their sum.

>  The void keyword in the definition specifies that the function does not return any value.
---
Let's change the function and specify the return type to be an int:
```
int sum(int x, int y) {
    
}
```
> This means that now our sum function will return an integer value.
---
Returning a Value
---
Now, we can return our result using the return keyword:
```
int sum(int x, int y) {
    return (x+y);
}
```
> The return keyword stops the function from executing. If there are any statements after return, they won't run.
---
After we have created our function, that returns a value, we can call it in our code and assign the result to a variable:
```
int result;
result = sum(21, 56);
cout << result;
```
> Returning is useful when you don't need to output the result of the function, but need to use it in your code.
For example, a bank account's withdraw() function could return the remaining balance of the account.
---
Lesson Takeaways
---
Now you know how to return values from functions!

Here is a quick summary:

- Use the return keyword to return a value from your function.
- The function needs to have its return type specified before its name.
- The void type specifies that the function does not return any value.
- The returned value can be assigned to a variable when calling the function.

We will learn about function overloading in the next lesson! It will be fun!