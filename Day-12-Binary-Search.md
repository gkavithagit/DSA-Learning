Day 12: Binary Search

Overview

Binary Search is an efficient searching algorithm used to find a target element in sorted data. It repeatedly divides the search range into half until the target is found or the range becomes empty.

How It Works

1. Initialize "left = 0".
2. Initialize "right = len(arr) - 1".
3. Calculate the middle index using "(left + right) // 2".
4. If the middle element equals the target, return its index.
5. If the target is greater than the middle element, search the right half.
6. Otherwise, search the left half.
7. Repeat until the target is found or the search range is empty.

Python Implementation

def binary_search(arr, target):
    left = 0
    right = len(arr) - 1

    while left <= right:
        mid = (left + right) // 2

        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1

    return -1


arr = [3, 7, 11, 15, 19, 23, 27, 31, 35]
target = 27

result = binary_search(arr, target)
print("Target index:", result)

Output

Target index: 6

Time and Space Complexity

- Best-case time complexity: O(1)
- Average-case time complexity: O(log n)
- Worst-case time complexity: O(log n)
- Auxiliary space complexity: O(1)

Key Takeaways

- Binary Search requires sorted data in its standard form.
- The middle element determines which half to search.
- "left" and "right" define the current search range.
- Python list indexing starts at zero.
- Binary Search is generally more efficient than Linear Search on large, sorted arrays.

Learning Outcome

Practiced Binary Search fundamentals, calculated middle indices, traced search operations, and reviewed time and space complexity.

Day 12 Status: Completed
