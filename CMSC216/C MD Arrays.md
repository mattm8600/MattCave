**Multi-Dimensional Arrays** store elements in *row major* order
- Starts at the `arr[0][0]`, go to `arr[0][i]`, then start the next left subscript
- Basically stores each array subscript in a long line

Name of [[C 1D Arrays]] are pointers to the element type
- Array name points to the first array (same as `arr[0]`)

### Ex: `arr[5][6]`
`*(arr+1)` → Points to the second array of six elements
`*(arr + 1) + 5` → Points to fifth element second array

### Pointer to MD Array
```
type (*p)[right size] = matrix;

int matrix[3][10];
int (*mp)[10] = matrix;
```
- pointer points to array of ten integers, pointer arithmetic now scales by the proper amount

To advance their arra