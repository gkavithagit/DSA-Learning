DSA Day 10: Sorting Algorithms — Bubble Sort

📌 Overview

Today, I learned the fundamentals of sorting algorithms and explored Bubble Sort, a beginner-friendly sorting algorithm used to arrange elements in ascending or descending order.

1. What Is Sorting?

Sorting is the process of arranging data in a specific order.

Example:

Before sorting:
"[5, 2, 4, 1]"

After sorting:
"[1, 2, 4, 5]"

Sorting helps organize data and is an important concept in Data Structures and Algorithms.

2. What Is Bubble Sort?

Bubble Sort repeatedly compares adjacent elements and swaps them if they are in the wrong order.

How It Works

1. Compare two adjacent elements.
2. Swap them if the left element is greater than the right element.
3. Continue comparing adjacent elements.
4. Repeat passes until the array is sorted.

Example:

Initial array: "[5, 2, 4, 1]"

After the first pass: "[2, 4, 1, 5]"

After the second pass: "[2, 1, 4, 5]"

Final sorted array: "[1, 2, 4, 5]"

3. Python Implementation

arr = [5, 2, 4, 1]

n = len(arr)

for i in range(n):
    for j in range(n - i - 1):
        if arr[j] > arr[j + 1]:
            arr[j], arr[j + 1] = arr[j + 1], arr[j]

print(arr)

Output:

[1, 2, 4, 5]

4. Time and Space Complexity

Case| Time Complexity
Best case| O(n²) for this implementation
Average case| O(n²)
Worst case| O(n²)

Auxiliary Space Complexity: O(1)

Note: An optimized Bubble Sort can achieve O(n) best-case time by stopping when a complete pass makes no swaps.

5. Advantages and Limitations

Advantages

- Easy to understand and implement.
- Requires constant auxiliary space.
- Useful for learning sorting fundamentals.

Limitations

- Inefficient for large datasets.
- Performs many comparisons and swaps.
- More efficient sorting algorithms are generally preferred in practice.

6. Key Takeaways

- Sorting arranges data in a particular order.
- Bubble Sort compares adjacent elements.
- The largest element moves to its final position after each complete pass in ascending-order sorting.
- The basic implementation has O(n²) time complexity in all cases.
- Its auxiliary space complexity is O(1).

7. Learning Progress

- [x] Learned sorting fundamentals.
- [x] Understood Bubble Sort logic.
- [x] Implemented Bubble Sort in Python.
- [x] Studied time and space complexity.
- [x] Completed the Day 10 concept quiz.
