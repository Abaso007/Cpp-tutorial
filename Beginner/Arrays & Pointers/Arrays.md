Arrays
---
Imagine working on a shopping app. Your program will need to store and work with multiple products and their prices. 
Instead of creating separate variables for each price, we can use an array to store all values!
><font color="#AE8E00">An array stores multiple values in a single variable.</font>
---
An array needs to be declared like a variable, with the type of the items it will hold.
```
double prices[5];
```
The name of the array is prices. It is created to hold 5 double values.

---
After declaring the array, we can access the items using their position, also called the index.
Let's set the item with the index 3 to the value 29.99:
```
prices[3] = 29.99;
```
><font color="#AE8E00">The index is specified in square brackets, next to the array name.</font>
---
The item with index 3 is actually the 4th item of the array. 
That's because array indexes start from 0, meaning that the first element's index is 0 rather than 1. 
Let's set the first item’s value:
```
prices[0] = 9.5;
```
><font color="#AE8E00">The last item of the prices array will have the index 7, as it can hold 8 items.</font>
---
Similarly, we can access the value of an item using its index:
```
cout << prices[3];
```
><font color="#AE8E00">This will output the value of the 4th item.</font>
---
If you already know what values to store in the array, instead of assigning them one by one, you can use the following syntax:
```
double prices[] = {5.99, 3.2, 9.99, 29.99};
```
Place the values in a comma-separated list, enclosed in curly braces. 
The code above automatically creates an array containing 4 items, and stores the provided values.
><font color="#AE8E00">When creating an array using this syntax, you can omit specifying the size in the square brackets, as it will be automatically set based on the number of values provided.</font>
---
Lesson Takeaways
---
Awesome! Here are some key points about arrays:
Arrays allow to store multiple values in a single variable.
When creating an array, we need to provide the type of the items and the size of the array, like this:
```
int numbers[15];
```
Array items are accessed using their indexes, placed in square brackets. The first item has the index 0.
You can also create an array with values using the following syntax, initializing its values:
```
int numbers[] = {1, 2, 3, 4, 5};
```
In the next lesson we will learn how to loop over the values of an array and make calculations.