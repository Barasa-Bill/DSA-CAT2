Q1.md
No 1. Ignore Constants
Big O notation focuses on growth rate, so constant factors are ignored.

An example is like:
5n+10 is O(n)
100n+500 is also O(n)
Even though the second function has larger constants, both grow linearly.

No 2. Drop Non-Dominant Terms
When multiple terms exist, only the fastest-growing one matters.

Example:
 n2+3n+7 is O(n²)
 n3+n2+n is O(n³)
Lower-order terms become insignificant as n grows.

No 3. Different Inputs, Different Variables
If an algorithm processes two independent inputs, use different variables.

Example:
If a function processes two lists, one of size m and another of size n, the complexity is O(m + n), not O(n).

 No 4. Nested Loops Multiply Complexity
When loops are nested, their complexities are multiplied.

Example:
A loop inside another loop running n times each results in O(n²).
If three nested loops run n times each, the complexity is O(n³).

No 5. Recursive Functions Follow Recurrence Relations
Recursive functions often have logarithmic or exponential complexity.
 
Example:
If a recursive function reduces the problem size by half each time, its complexity is O(log n) (like binary search).
If a function splits into two calls each time, it results in O(2ⁿ) (like Fibonacci).


Q2.md
(i) Memory Allocation -In arrays memory is allocated in a continuous block whereas in linked list memory is allocated dynamically in non-contiguous locations.
(ii) Performance - Arrays in terms of access speed, fast access to elements by index is required directly O(1) whereas linked list, sequential access is required O(n) 
(iii). Insertion and Deletion : In arrays, Insertions and deletions are infrequent and mostly at the end whereas Linked lists, Frequent insertions and deletions are needed, especially at the beginning or middle.
