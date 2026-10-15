Day 15: Binary Search Practice and Applications

📌 Overview

Today, I revised Binary Search and focused on understanding how it works, when to use it, and how it helps solve placement-oriented programming problems efficiently.

🎯 Learning Objectives

- Revise the Binary Search algorithm.
- Understand the "low", "high", and "mid" variables.
- Learn how to update the search range.
- Understand the conditions for searching the left and right halves.
- Analyze the time and auxiliary space complexities.
- Explore common applications of Binary Search in coding interviews.

🔍 What Is Binary Search?

Binary Search is an efficient searching algorithm that repeatedly divides a search range into two halves to find a target element.

Important condition: Standard Binary Search requires a sorted array.

⚙️ How Binary Search Works

1. Initialize "low = 0".
2. Initialize "high = len(arr) - 1".
3. Calculate the middle index using "mid = (low + high) // 2".
4. Compare the middle element with the target.
5. If they are equal, return the middle index.
6. If the middle element is smaller than the target, search the right half.
7. If the middle element is larger than the target, search the left half.
8. Repeat until the target is found or the search range becomes empty.

💻 Example

arr = [2, 5, 8, 12, 16, 23, 38]
target = 16

low = 0
high = len(arr) - 1

while low <= high:
    mid = (low + high) // 2

    if arr[mid] == target:
        print("Element found at index:", mid)
        break
    elif arr[mid] < target:
        low = mid + 1
    else:
        high = mid - 1
else:
    print("Element not found")

Output:

Element found at index: 4

⏱️ Time and Space Complexity

Case| Complexity
Best-case time| O(1)
Average-case time| O(log n)
Worst-case time| O(log n)
Auxiliary space (iterative)| O(1)

🚀 Applications of Binary Search

- Searching for an element in a sorted array.
- Finding the first or last occurrence of an element.
- Finding the insertion position of an element.
- Solving search-space problems using Binary Search techniques.

💡 Key Takeaways

- Binary Search works by repeatedly reducing the search range.
- Standard Binary Search requires sorted data.
- Updating "low" and "high" correctly is essential.
- Binary Search has O(log n) worst-case time complexity.
- Iterative Binary Search uses O(1) auxiliary space.

📈 Day 15 Progress

Topic: Binary Search — Practice and Applications
Focus: Algorithm revision, search-range updates, complexity analysis, and placement preparation.


#DSA #Python #BinarySearch #100DaysOfCode #CodingPractice #PlacementPreparation
