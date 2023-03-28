Arrays
---
We can use a loop to iterate over the items of an array.
For example, let's simply output all the items using a for loop:
```
double prices[] = {5.99, 3.2, 9.99, 29.99};

for(int i=0;i<4;i++) {
  cout << prices[i] << endl;
}
```
We used the i variable of the loop as the index for our array. During each iteration of the loop it is incremented and used to access the corresponding item of the array.

---
We can also use loops to perform calculations with arrays.
For example, let's calculate the sum of all values of the prices array:
```
double prices[] = {5.99, 3.2, 9.99, 29.99};

double total=0;
for(int i=0;i<4;i++) {
  total += prices[i];
}
cout << total;
```
In the code above, we declared a variable total to store the result and assigned it 0.
Then, in the for loop, we added the value of each item of the array to it.

---
To make iterating over arrays easier and shorter, C++ provides another type of the for loop, called the for-each loop.
Here is an example:
```
double prices[] = {5.99, 3.2, 9.99, 29.99};

for(double x: prices) {
  cout << x << endl;
}
```
Цикл создает переменную, которая автоматически присваивается каждому значению массива во время цикла.
Мы назвали его xв нашем примере, но вы можете назвать его как угодно.

><font color="#AE8E00">Обратите внимание на двоеточие после переменной — оно читается как « для каждого x в ценах ».</font>
---
Remember the auto keyword? It was used to automatically set the type of a variable based on the value it is assigned to.
We can also use the auto keyword in a for-each loop:
```
for(auto x: prices) {
  cout << x << endl;
}
```
Now, the code will work for any type of arrays.

---
Lesson Takeaways
---
Now you know how to loop over arrays.
You can use a for loop to loop over an array.
For example, for an array called arr of 5 items:
```
for(int x=0;x<5; x++) {
   //current item is arr[x]
}
```
Another way to loop over arrays is the for-each loop:
```
for(auto x: arr) {
  //current item is x
}
```
The auto keyword automatically takes the type of the item's value.
We will learn about multidimensional arrays in the next lesson!
