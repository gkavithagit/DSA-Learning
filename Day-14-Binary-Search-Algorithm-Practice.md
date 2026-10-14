📅 Day 14: Binary Search — Algorithm Practice

🎯 Learning Objectives

- Revised the fundamentals of Binary Search.
- Understood how to identify the middle element.
- Learned how to eliminate half of the search space in each iteration.
- Practiced Binary Search logic using Python.
- Reviewed time complexity and array indexing.

📚 Concepts Learned

1. Binary Search

Binary Search is an efficient searching algorithm that repeatedly divides a sorted search space into halves to locate a target element.

2. Algorithm Steps

1. Initialize "left = 0".
2. Initialize "right = len(arr) - 1".
3. Calculate the middle index using "(left + right) // 2".
4. If the middle element equals the target, return its index.
5. If the target is greater than the middle element, search the right half.
6. If the target is smaller than the middle element, search the left half.
7. If the target is not found, return "-1".

3. Python Implementation

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


numbers = [10, 20, 30, 40, 50, 60, 70]

print(binary_search(numbers, 50))

Output:

4

⏱️ Time Complexity

- Best Case: O(1)
- Average Case: O(log n)
- Worst Case: O(log n)

💾 Space Complexity

- Auxiliary Space: O(1) for this iterative implementation.

⚠️ Important Note

Standard Binary Search requires sorted data. It is significantly more efficient than Linear Search for large sorted arrays.

📝 Practice Completed

- Binary Search concept revision.
- Middle element identification.
- Search direction determination.
- Array indexing practice.
- Time complexity MCQ quiz: 5/5.

🚀 Key Takeaway

Today, I strengthened my understanding of Binary Search and learned how its divide-and-conquer approach reduces the search space efficiently.

Next Goal: Improve problem-solving skills by implementing searching algorithms independently and solving coding problems.

#DSA #Python #BinarySearch #ProblemSolving #100DaysOfCode
