Day 30 – Move Zeroes

📌 Problem Statement

Given an integer array, move all zeroes to the end of the array while maintaining the relative order of all non-zero elements.

Example

Input:

arr = [0, 1, 0, 3, 12]

Output:

[1, 3, 12, 0, 0]

Concepts Learned

- Array Traversal
- Array Manipulation
- Two Pointer Technique
- In-place Modification
- Time and Space Complexity

Approach 1: Using an Additional Array

1. Create an empty result array.
2. Traverse the original array.
3. Append all non-zero elements.
4. Count the zeroes.
5. Append the required number of zeroes at the end.

Time Complexity: O(n)
Space Complexity: O(n)

Approach 2: Optimized Two Pointer Technique

1. Initialize "pos = 0".
2. Traverse the array using index "i".
3. Check whether the current element is non-zero.
4. If non-zero, swap "arr[i]" with "arr[pos]".
5. Increment "pos".
6. Continue until the array traversal is complete.

Time Complexity: O(n)
Auxiliary Space Complexity: O(1)

Python Implementation

arr = [0, 1, 0, 3, 12]

pos = 0

for i in range(len(arr)):
    if arr[i] != 0:
        arr[pos], arr[i] = arr[i], arr[pos]
        pos += 1

print(arr)

Output:

[1, 3, 12, 0, 0]

Key Takeaway

The Two Pointer Technique helps solve array manipulation problems efficiently. It allows us to modify the original array without requiring additional storage.

🎯 Learning Outcome

Completed Day 30 of my DSA learning journey and strengthened my understanding of array manipulation, optimized approaches, and in-place algorithms.
