DSA Day 19: First and Last Occurrence Using Binary Search

📌 Today's Learning

Today, I learned how to find the first and last occurrences of a target element in a sorted array using Binary Search.

1. What Is First Occurrence?

The first occurrence is the smallest index at which the target element appears in the array.

Example:

arr = [1, 2, 4, 4, 4, 4, 5, 6]
target = 4

First occurrence of 4 = Index 2.

2. What Is Last Occurrence?

The last occurrence is the largest index at which the target element appears in the array.

Example:

arr = [1, 2, 4, 4, 4, 4, 5, 6]
target = 4

Last occurrence of 4 = Index 5.

3. Count Occurrences

When the first and last occurrences are known, we can calculate the total number of occurrences using this formula:

Count = Last Occurrence - First Occurrence + 1

Example:

- First occurrence = 2
- Last occurrence = 5
- Count = 5 - 2 + 1 = 4

Therefore, the target element appears 4 times.

4. Binary Search Logic

To find the first occurrence:

1. Apply binary search.
2. If the middle element equals the target, store its index.
3. Continue searching the left half.
4. Return the earliest recorded index.

To find the last occurrence:

1. Apply binary search.
2. If the middle element equals the target, store its index.
3. Continue searching the right half.
4. Return the latest recorded index.

5. Time and Space Complexity

- Time Complexity: O(log n) for each binary search.
- Auxiliary Space Complexity: O(1) for an iterative implementation.

Finding both occurrences takes O(log n) time overall.

6. Important Notes

- Binary search requires a sorted array.
- Array indexing starts at 0 in Python.
- The "+1" in the counting formula includes both the first and last positions.
- If the target does not exist, its occurrence count is 0.

🎯 Day 19 Outcome

I learned the concepts behind finding the first and last occurrences of an element, counting duplicates, and applying binary search logic.

Status: Day 19 Completed ✅

#DSA #BinarySearch #Python #ProblemSolving #CodingInterview
