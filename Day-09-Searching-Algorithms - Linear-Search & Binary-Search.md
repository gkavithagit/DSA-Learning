Day 09: Searching Algorithms — Linear Search & Binary Search

📌 Overview

Today, I learned two fundamental searching algorithms in Data Structures and Algorithms (DSA): Linear Search and Binary Search.

The goal was to understand how searching algorithms work, compare their time complexities, and identify when to use each algorithm.

🎯 Topics Covered

1. Linear Search

Linear Search checks each element sequentially until the target element is found or the array ends.

Key Concepts:

- Works with sorted and unsorted arrays.
- Uses loops and conditional statements.
- Best-case time complexity: O(1).
- Average-case time complexity: O(n).
- Worst-case time complexity: O(n).

Python Implementation:

arr = [10, 25, 30, 45, 60]
target = 45

for i in range(len(arr)):
    if arr[i] == target:
        print("Found at index:", i)
        break

Output:

Found at index: 3

2. Binary Search

Binary Search repeatedly divides the search interval into halves to locate a target element.

Key Concepts:

- Requires sorted data for standard Binary Search.
- Uses "left", "right", and "mid" pointers.
- Eliminates half of the remaining search interval after each unsuccessful comparison.
- Best-case time complexity: O(1).
- Average-case time complexity: O(log n).
- Worst-case time complexity: O(log n).

Python Implementation:

arr = [10, 20, 30, 40, 50, 60, 70]
target = 60

left = 0
right = len(arr) - 1

while left <= right:
    mid = (left + right) // 2

    if arr[mid] == target:
        print("Found at index:", mid)
        break
    elif arr[mid] < target:
        left = mid + 1
    else:
        right = mid - 1

Output:

Found at index: 5

📊 Linear Search vs Binary Search

Feature| Linear Search| Binary Search
Searching approach| Sequential| Divide and conquer
Requires sorted data| No| Yes
Best-case time| O(1)| O(1)
Average-case time| O(n)| O(log n)
Worst-case time| O(n)| O(log n)

🧠 Key Learnings

- Understood the working principles of Linear Search and Binary Search.
- Learned why Binary Search requires sorted data.
- Practiced calculating the middle index using integer division.
- Improved my understanding of algorithmic time complexity.
- Learned that algorithm selection depends on the input data and problem requirements.

🎯 Placement Preparation

Searching algorithms are fundamental DSA topics frequently used in coding practice and technical interview preparation.

My next goal is to strengthen my implementation skills, solve searching problems independently, and improve my ability to analyze algorithm efficiency.

📅 Learning Progress

DSA Day: 09
Topic: Searching Algorithms
Language: Python
Focus: Algorithm implementation, time complexity, and problem-solving.

