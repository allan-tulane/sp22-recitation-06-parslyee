# CMPS 2200 Reciation 6
## Answers

**Name:**Lily Yee


Place all written answers from `recitation-06.md` here for easier grading.







- **1b.**

Random:

  n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|---------------------|----------------------|
|   5 |               0.019 |                0.019 |
|  10 |               0.026 |                0.033 |
|  15 |               0.039 |                0.057 |
| 100 |               0.304 |                0.411 |
| 150 |               0.478 |                0.648 |
| 200 |               0.906 |                0.960 |
| 250 |               0.888 |                1.109 |
| 300 |               1.133 |                1.372 |
| 350 |               1.253 |                1.676 |
| 400 |               1.492 |                1.892 |
| 450 |               1.798 |                2.328 |
| 500 |               2.073 |                2.365 |

Sorted:

|   n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|---------------------|----------------------|
|   5 |               0.022 |                0.040 |
|  10 |               0.029 |                1.610 |
|  15 |               0.051 |                0.052 |
| 100 |               1.341 |                0.410 |
| 150 |               2.668 |                0.687 |
| 200 |               4.208 |                0.837 |
| 250 |               6.766 |                1.086 |
| 300 |               9.751 |                1.362 |
| 350 |              13.136 |                1.569 |
| 400 |              17.870 |                1.889 |
| 450 |              23.509 |                2.171 |
| 500 |              26.012 |                2.441 |

Using a sorted list with a fixed pivot is not efficient when compared to the other results, especially as list size increases. When the list is randomized, it is much more efficient and that can be seen with improved runtimes. It's hard to determine a trend from any of the results, but it is clear that the least efficient method with the slowest runtime is using a sorted list with a fixed pivot, and overall using a randomized list has a lower runtime and is more efficient than using a sorted list. 




- **1c.**

Random:

|   n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sort |
|-----|---------------------|----------------------|------------|
|   5 |               0.019 |                0.020 |      0.002 |
|  10 |               0.026 |                0.235 |      0.002 |
|  15 |               0.041 |                0.051 |      0.001 |
| 100 |               0.328 |                0.439 |      0.010 |
| 150 |               0.542 |                0.715 |      0.015 |
| 200 |               0.703 |                0.951 |      0.026 |
| 250 |               0.928 |                1.173 |      0.026 |
| 300 |               1.086 |                1.308 |      0.031 |
| 350 |               1.704 |                2.065 |      0.039 |
| 400 |               1.558 |                2.478 |      0.049 |
| 450 |               1.773 |                2.194 |      0.048 |
| 500 |               2.694 |                2.563 |      0.058 |

Sorted:

|   n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sort |
|-----|---------------------|----------------------|------------|
|   5 |               0.019 |                0.025 |      0.002 |
|  10 |               0.030 |                0.050 |      0.001 |
|  15 |               0.053 |                0.052 |      0.001 |
| 100 |               1.371 |                0.419 |      0.002 |
| 150 |               2.462 |                0.621 |      0.003 |
| 200 |               4.631 |                0.957 |      0.005 |
| 250 |               7.031 |                1.149 |      0.006 |
| 300 |               9.760 |                1.337 |      0.006 |
| 350 |              12.914 |                1.625 |      0.005 |
| 400 |              18.002 |                1.948 |      0.007 |
| 450 |              23.883 |                2.279 |      0.007 |
| 500 |              26.545 |                2.377 |      0.007 |

The trends for both implementations of qsort are similar to the trends in 1b. tim_sort is faster than both implementations, and especially when compared to the two implementations when using a sorted list. tim_sort has the fastest runtime and is the most efficient. 
