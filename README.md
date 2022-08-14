# pssort
array sort for postscript

<hr>

This repository contains 2 sort functions fpr PostScript:
- mergesort.ps
- quicksort.ps

Each function takes 2 parameters:
1. an array
2. a code block for comparison of 2 array elements

[C B A] {cmp}  **mergesort**/**quicksort**  [A B C] {cmp}

### Use case
There are 2 functions for a more convenient use
- arraysort - sorts an array of comarable items (numbers, strings)
- dictsort - converts a dictionary into an array with each key/value pair becoming a 2 element array.

### Sort Order
The sort order is **ascending**. It can be changed by customizing the functions **cmp** and **cmpdict**
```
lt --> gt
```

### Performance
On my AMD Ryzen 5 3600 to sort an array with 1 million numbers it takes for
- mergesort: 4.07 seconds
- quicksort: 5.38 seconds
