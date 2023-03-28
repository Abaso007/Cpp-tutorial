Arrays
---
In the previous lessons we have seen arrays with a fixed size.
Their size needed to be defined when they were created using a constant number.
What if we needed an array that has a size that is a variable? 
For example, imagine a program that takes an image as input and processes it using an array. The image size is only known when the program runs, so we do not know in advance what the size of the array will be.
In these situations we need to dynamically allocate memory. Let's learn how to do that!

---
Pointers
---
In order to learn about dynamic memory, we first need to learn about pointers.
All variables that you create are stored in the memory. 
A pointer is a variable that stores the memory address of another variable as its value.
It is defined using the asterisk sign and is defined just like a variable:
```
int *p;
```
><font color="#AE8E00">Let's learn how to assign it a value!</font>
---
The address of a variable can be accessed using the & operator.
```
int num = 42;

int *p = &num;

cout << p;
```
The code above creates a pointer called p and assigns it the memory address of the variable num.
><font color="#AE8E00">Run the code to see the value of p. It is a long hexadecimal number that represents a memory address.</font>
---
The asterisk * is also used to access the value stored at a memory address. It is called the dereference operator.
Let's output the value stored at the address to which the pointer p points:
```
int *p = &num;

cout << *p;
```
This will output the value of the variable, to which the pointer points to.

><font color="#AE8E00">Remember the following:
>
>- The & operator is used to access the memory location of a variable.
>- The * operator is used to access the value of a memory address that is stored in a pointer.
>- The same * sign is also used to declare a pointer, and it is different from the dereference operator.</font>

---
Because the pointer points to the memory address of a variable, we can use it to change the value of that variable:
For example:
```
int num = 42;
int *p = &num;

*p = 8;
cout << num;
```
Run the code to see the result.
><font color="#AE8E00">We have changed the value of a variable using the pointer. 
*p is basically an alias for num, meaning that they represent the same thing. When you change the value of *p, num is also changed, and vice-e-versa, changing num will also change the value of *p.</font>

---
Arrays & Pointers
---
The name of an array is actually a pointer to its first element.
Each element can be accessed by incrementing the pointer.
Here is an example:
```
int arr[] = {2, 4, 6, 8};

int *p = arr;

// first element
cout << *p << endl;

// second element
cout << *(p+1) << endl;

// third element
cout << *(p+2) << endl;
```
Note, that we used *p = arr and not &arr. This is because the array name is already a pointer and is the same as &arr[0].

><font color="#AE8E00">Also, note that we used the dereference operator like this: *(p+1), so that it accessed the incremented address. The parentheses are important!</font>
---

We can use pointers to arrays to loop over them.
Here is an example:
```
int arr[] = {2, 4, 6, 8};

int *p = arr;

for(int i=0;i<4;i++) {
  cout << *p << endl;
  p++;
}
```
During each iteration of the loop we simply increment the pointer by 1, making it point to the next element of the array.

---
Lesson Takeaways
---
Pointers might seem confusing at first, but don't worry, you'll get the hang of it! Here are the key takeaways:

- A pointer is a variable that stores the memory address of another variable.
- It is declared using a * and the type of the value it points to, for example: int *p;
- The memory address of a variable can be accessed using the & operator, and assigned to a pointer, for example: int *p = & num;
- The value of a memory address can be accessed using the * operator, for example *p is the value stored at the address that p points to.
- A pointer can also be assigned to an array and be used to access the elements of the array, by simply incrementing the pointer.


We learned about pointers, because they are used for dynamic memory allocation, which we will cover in the next lesson!
