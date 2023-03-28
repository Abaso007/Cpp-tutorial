Dynamic Memory
---

Now that we know about pointers, let's learn how to create dynamic arrays (arrays which have a variable size). 
These are handy when we need to allocate new memory based on user input.
For example, let's say we have a size variable that takes a value dynamically, based on user input.
For simplicity of our example, we will just assign it a value:
```
int size = 8;
```
Now, we want to create an array of that size dynamically.

---
The new operator is used to allocate memory. It then can be assigned to a pointer.
For example:
```
int size = 8;

int * p = new int[size];
```

><font color="#AE8E00">Now, p hold the address of our newly allocated memory, which can be used to store 8 item, because size = 8;</font>

---
Now, we can use our pointer to assign values and access them:
```
int size = 8;

int *p = new int[size];

p[0] = 128;
p[1] = 888;
p[2] = 9;

cout << *(p+1);
```

---
We can also use size in a for loop, as the condition.
Let's assign the number 1 to size to the array elements, then output them:
```
int size = 8;

    int *p = new int[size];

    for(int i=0;i<size;i++) {
        p[i] = i;
    }

    for(int i=0;i<size;i++) {
       cout << p[i] << endl;
    }

```


><font color="#AE8E00">You can change the value of size, and see how the same code works for any given value.</font>
---
In most cases, memory allocated dynamically is only needed during specific periods of time within a program; once it is no longer needed, it can be freed so that the memory becomes available again for other requests of dynamic memory.
This is the purpose of the delete operator:
```
delete[] p;
```

><font color="#AE8E00">This frees up the memory taken by the array p.</font>
---
Lesson Takeaways
---
Dynamic memory allocation is useful in many situations, such as when your program depends on input. As an example, when your program needs to read an image file, it doesn't know in advance the size of the image file and the memory necessary to store the image.

- Memory is allocated using the new keyword: int* p = new int[size];
- After the allocated memory is no longer needed, we can free it up using delete: delete[] p;