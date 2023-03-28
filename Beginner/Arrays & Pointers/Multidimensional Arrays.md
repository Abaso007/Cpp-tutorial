Multidimensional Arrays
---
An array can have multiple dimensions (or indices) to represent a grid.
For example, imagine a movie theater program that is storing the seats, which have a row and column number.
Or a game board/map, where each square has 2 coordinates.

><font color="#AE8E00">The arrays in the examples would have 2 dimensions.</font>
---
To create multidimensional arrays, place each array within its own set of square brackets:
```
int seats[2][3] =
    {
    {1, 2, 3}, 
    {4, 5, 6}
    };
```

><font color="#AE8E00">The array has two dimensions: 2 rows and 3 columns.</font>
---

The elements are accessed by using the row index and column index of the array.
For example, let's output the 3rd item of the 2nd array:

```
int seats[2][3] = {{1, 2, 3}, {4, 5, 6}};

cout << seats[1][2];
```
The first index accesses the 2nd array, while the second index accesses the 3rd item in it.

---
Indices for two-dimensional arrays are also called row and column indices.
We can format the code in the following way to make it easier to read:
```
int seats[2][3] = {
  {1, 2, 3}, 
  {4, 5, 6}
};
```
Each row is an item, which is an array. So, to access a value, we provide the row index, then the column index.

---
We can loop over a two-dimensional array using nested for loops:
```
for(int i=0;i<2;i++) {
  for(int j=0;j<3;j++) {
    cout << seats[i][j] << endl;
  }
}
```
The first loop iterates over the rows, the second one over their items.

---
Lesson Takeaways
---
Arrays with multiple dimensions are simply arrays that contain other arrays.
The number of square brackets match the dimension of the array, for example [][] denotes a 2-dimensional array.
To access the items of the array, specify the row index in the first square brackets, followed by the column index in the second.




