Day 29: Merge Two Sorted Arrays

📌 Overview

Today's topic focuses on merging two sorted arrays into a single sorted array using Python. The main objective is to understand how the Two-Pointer Technique can reduce unnecessary sorting operations and improve efficiency.

🎯 Learning Objectives

- Understand the problem of merging two sorted arrays.
- Implement a basic solution using Python's built-in sorting functionality.
- Apply the Two-Pointer Technique to merge arrays efficiently.
- Handle remaining elements when one array is exhausted.
- Analyze time and space complexity.

🧩 Problem Statement

Given two arrays sorted in ascending order, merge them into one sorted array.

Example:

Input:

arr1 = [1, 3, 5]
arr2 = [2, 4, 6]

Output:

[1, 2, 3, 4, 5, 6]

💡 Approach 1: Combine and Sort

Code

arr1 = [1, 3, 5]
arr2 = [2, 4, 6]

result = sorted(arr1 + arr2)
print(result)

Complexity Analysis

- Time Complexity: O((n + m) log(n + m))
- Auxiliary Space Complexity: O(n + m), excluding implementation-dependent sorting overhead.

This approach is easy to understand but performs an additional sorting operation.

⚡ Approach 2: Two-Pointer Technique

Logic

1. Initialize two pointers at the beginning of the arrays.
2. Compare the elements at the current pointer positions.
3. Append the smaller element to the result.
4. Move the corresponding pointer forward.
5. Continue until one array is exhausted.
6. Append the remaining elements from both arrays, if any.

Code

def merge_sorted_arrays(arr1, arr2):
    i = 0
    j = 0
    result = []

    while i < len(arr1) and j < len(arr2):
        if arr1[i] < arr2[j]:
            result.append(arr1[i])
            i += 1
        else:
            result.append(arr2[j])
            j += 1

    result.extend(arr1[i:])
    result.extend(arr2[j:])

    return result


arr1 = [1, 3, 5]
arr2 = [2, 4, 6]

print(merge_sorted_arrays(arr1, arr2))

Output

[1, 2, 3, 4, 5, 6]

Complexity Analysis

- Time Complexity: O(n + m)
- Auxiliary Space Complexity: O(n + m) for the result array.

Here, "n" and "m" represent the lengths of the two input arrays.

🔍 Key Concepts Learned

- Array traversal
- Two-Pointer Technique
- Conditional comparisons
- Python list methods: "append()" and "extend()"
- Time and space complexity
- Efficient merging of sorted data

📝 Day 29 Summary

Learned how to merge two sorted arrays using both a straightforward sorting approach and the more efficient Two-Pointer Technique.

The key takeaway is that when input arrays are already sorted, their existing order can be used to merge them in linear time.

🚀 Next Practice Goal

Extend the solution to merge two sorted arrays while removing duplicate values, without using "set()" or "sorted()".

Progress: Day 29 completed — Merge Two Sorted Arrays.
