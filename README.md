![Image](https://gifimage.net/wp-content/uploads/2018/11/merge-sort-animation-gif-5.gif)
# Merge-Sort
In computer science, merge sort (also commonly spelled as mergesort) is an efficient, general-purpose, and comparison-based sorting algorithm. Most implementations produce a stable sort, which means that the order of equal elements is the same in the input and output. Merge sort is a divide and conquer algorithm that was invented by John von Neumann in 1945. A detailed description and analysis of bottom-up merge sort appeared in a report by Goldstine and von Neumann as early as 1948.

Conceptually, merge sort works as follows:

1. Divide the unsorted list into n sublists, each containing one element (a list of one element is considered sorted).
2. Repeatedly merge sublists to produce new sorted sublists until there is only one sublist remaining. This will be the sorted list.


Analysis

A recursive merge sort algorithm used to sort an array of 7 integer values. These are the steps a human would take to emulate merge sort (top-down).
In sorting n objects, merge sort has an average and worst-case performance of O(n log n). If the running time of merge sort for a list of length n is T(n), then the recurrence relation T(n) = 2T(n/2) + n follows from the definition of the algorithm (apply the algorithm to two lists of half the size of the original list, and add the n steps taken to merge the resulting two lists).[5] The closed form follows from the master theorem for divide-and-conquer recurrences.

![Image](https://upload.wikimedia.org/wikipedia/commons/e/e6/Merge_sort_algorithm_diagram.svg)

The number of comparisons made by merge sort in the worst case is given by the sorting numbers. These numbers are equal to or slightly smaller than (n ⌈lg n⌉ − 2⌈lg n⌉ + 1), which is between (n lg n − n + 1) and (n lg n + n + O(lg n)).[6] Merge sort's best case takes about half as many iterations as its worst case.[7]

For large n and a randomly ordered input list, merge sort's expected (average) number of comparisons approaches α·n fewer than the worst case, where {\displaystyle \alpha =-1+\sum _{k=0}^{\infty }{\frac {1}{2^{k}+1}}\approx 0.2645.}\alpha =-1+\sum _{k=0}^{\infty }{\frac {1}{2^{k}+1}}\approx 0.2645.

In the worst case, merge sort uses approximately 39% fewer comparisons than quicksort does in its average case, and in terms of moves, merge sort's worst case complexity is O(n log n) - the same complexity as quicksort's best case.[7]

Merge sort is more efficient than quicksort for some types of lists if the data to be sorted can only be efficiently accessed sequentially, and is thus popular in languages such as Lisp, where sequentially accessed data structures are very common. Unlike some (efficient) implementations of quicksort, merge sort is a stable sort.

Merge sort's most common implementation does not sort in place;[8] therefore, the memory size of the input must be allocated for the sorted output to be stored in (see below for variations that need only n/2 extra spaces).


# Complexity Analysis of Merge Sort
Merge Sort is quite fast, and has a time complexity of O(n*log n). It is also a stable sort, which means the "equal" elements are ordered in the same order in the sorted list.

## why the running time for merge sort is O(n*log n)?

In Binary Search whenever we divide a number into half in every step, it can be represented using a logarithmic function, which is log n and the number of steps can be represented by log n + 1(at most)

Also, we perform a single step operation to find out the middle of any subarray, i.e. O(1).

And to merge the subarrays, made by dividing the original array of n elements, a running time of O(n) will be required.

Hence the total time for mergeSort function will become n(log n + 1), which gives us a time complexity of O(n*log n).

Worst Case Time Complexity [ Big-O ]: O(n*log n)

Best Case Time Complexity [Big-omega]: O(n*log n)

Average Time Complexity [Big-theta]: O(n*log n)

## Space Complexity: O(n)

Time complexity of Merge Sort is O(n*Log n) in all the 3 cases (worst, average and best) as merge sort always divides the array in two halves and takes linear time to merge two halves. It requires equal amount of additional space as the unsorted array. Hence its not at all recommended for searching large unsorted arrays.
It is the best Sorting technique used for sorting Linked Lists.



|      Name               | ID Number       |
| ----------------------  | --------------- |
| 1.Henok Biadglign       | CNCS/UR15201/12 |
| 2.Hailemariam Desalegn  | CNCS/UR15176/12 |
| 3.Biniyam Tamene        | CNCS/UR15014/12 |
| 4.Bitanya Gizate        | CNCS/UR15033/12 |
| 5.Kibruyisfa Dinkayehu  | CNCS/UR15239/12 |
| 6.Sossna Zerfu          | CNCS/UR15466/12 |

