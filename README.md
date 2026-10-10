🚀 Data Structures and Algorithms (DSA) Learning Journey with Python

Welcome to my Data Structures and Algorithms (DSA) Learning Repository!

I'm a second-year B.Sc. Computer Science student specializing in Cybersecurity, building a strong foundation in problem-solving, algorithm design, and Python programming to prepare for software development and cybersecurity-related placements.

This repository documents my daily DSA learning journey, including core concepts, Python implementations, complexity analysis, practice questions, and key takeaways.

My goal is to understand how algorithms work, analyze their efficiency, and develop the ability to solve coding problems independently.

---

🎯 Learning Objectives

- Build a strong foundation in Data Structures and Algorithms.
- Improve logical thinking and problem-solving skills.
- Understand time and space complexity.
- Implement fundamental algorithms using Python.
- Develop efficient approaches to coding problems.
- Prepare for technical interviews and placement assessments.
- Maintain a consistent learning record through GitHub.

---

📚 Daily Learning Progress

✅ Day 1 — Introduction to DSA

Topics Covered:

- Introduction to Data Structures and Algorithms.
- Importance of DSA in programming and software development.
- Understanding how data structures organize data.
- Understanding how algorithms solve problems.
- Introduction to the DSA learning roadmap.

Key Takeaway:

Data structures organize and store data, while algorithms define the steps used to process data and solve problems.

---

✅ Day 2 — Time Complexity and Big O Notation

Topics Covered:

- Introduction to time complexity.
- Understanding Big O notation.
- Analyzing how an algorithm's running time grows with input size.
- Introduction to common complexity classes.

Complexities Studied:

Complexity| Meaning| Example
O(1)| Constant time| Accessing an array element by index
O(n)| Linear time| Traversing an array
O(n²)| Quadratic time| Comparing every pair in a simple nested-loop pattern

Key Takeaway:

Time complexity helps estimate how an algorithm's running time grows as the input size increases.

---

✅ Day 3 — Space Complexity

Topics Covered:

- Introduction to space complexity.
- Understanding memory usage as input size grows.
- Difference between total space and auxiliary space.
- Identifying additional variables and data structures used by algorithms.

Example:

def find_first(arr):
    if arr:
        return arr[0]
    return None

The function uses O(1) auxiliary space because it requires only a constant amount of additional memory.

Key Takeaway:

Space complexity helps evaluate the memory requirements of an algorithm.

---

✅ Day 4 — Auxiliary Space Complexity

Topics Covered:

- Understanding auxiliary space.
- Identifying extra memory used during execution.
- Distinguishing input storage from additional working memory.
- Analyzing variables and temporary data structures.

Example:

def calculate_sum(arr):
    total = 0

    for num in arr:
        total += num

    return total

Auxiliary Space: O(1)

The function uses a constant amount of additional memory, regardless of the number of elements in the input array.

Key Takeaway:

An algorithm can process a large input without necessarily requiring a large amount of auxiliary memory.

---

✅ Day 5 — Algorithm Analysis and Complexity Practice

Topics Covered:

- Practising time complexity analysis.
- Identifying common complexity patterns.
- Applying Big O concepts to code examples.
- Improving understanding of algorithm efficiency.

Key Takeaway:

Understanding how loops and repeated operations affect running time is an important step toward analyzing algorithms independently.

---

✅ Day 6 — Recursion Fundamentals

Topics Covered:

- Introduction to recursion.
- Understanding how a function calls itself.
- Identifying base cases.
- Understanding recursive calls.
- Learning why recursion must eventually reach a stopping condition.

Example:

def countdown(n):
    if n == 0:
        return

    print(n)
    countdown(n - 1)

countdown(3)

Output:

3
2
1

Key Takeaway:

Recursion solves a problem by breaking it into smaller versions of the same problem. A correct base case prevents infinite recursive calls.

---

✅ Day 7 — Arrays: Insertion, Deletion, and Complexity

Topics Covered:

- Understanding arrays and indexed access.
- Inserting elements into a list.
- Deleting elements from a list.
- Understanding why insertion and deletion can require shifting elements.
- Analysing operation complexity.

Example:

arr = [10, 20, 30, 40]

arr.insert(1, 15)
print(arr)

arr.pop(2)
print(arr)

Output:

[10, 15, 20, 30, 40]
[10, 15, 30, 40]

Complexity Notes:

Operation| Typical Complexity
Access by index| O(1)
Insert at the beginning| O(n)
Delete from the beginning| O(n)
Append to a Python list| O(1) amortized

Key Takeaway:

Array operations have different costs depending on where elements are inserted or deleted.

---

✅ Day 8 — Arrays: Practical Understanding

Topics Covered:

- Reviewing array fundamentals.
- Understanding array indexing.
- Analysing element access and traversal.
- Practising array-related questions.
- Connecting array operations with complexity analysis.

Key Takeaway:

Understanding indexing, traversal, and operation costs provides a foundation for solving more advanced array problems.

---

✅ Day 9 — Searching Algorithms

Topics Covered:

- Understanding the purpose of searching algorithms.
- Learning Linear Search.
- Learning Binary Search.
- Comparing their time complexities.
- Implementing searching algorithms using Python.

Linear Search

Checks elements one by one until the target is found or the collection ends.

Time Complexity:

- Best case: O(1)
- Average case: O(n)
- Worst case: O(n)

Binary Search

Repeatedly halves the search interval to find a target in a sorted array.

Time Complexity:

- Best case: O(1)
- Average case: O(log n)
- Worst case: O(log n)

Key Takeaway:

Linear Search works with sorted and unsorted arrays, while standard Binary Search requires sorted data. Binary Search is generally more efficient for searching large, sorted collections.

---

✅ Day 10 — Sorting Algorithms: Bubble Sort

Topics Covered:

- Introduction to sorting algorithms.
- Understanding Bubble Sort.
- Comparing adjacent elements.
- Swapping elements that are in the wrong order.
- Implementing Bubble Sort using Python.
- Analysing time and auxiliary space complexity.

Python Implementation:

arr = [5, 2, 4, 1]
n = len(arr)

for i in range(n):
    for j in range(n - i - 1):
        if arr[j] > arr[j + 1]:
            arr[j], arr[j + 1] = arr[j + 1], arr[j]

print(arr)

Output:

[1, 2, 4, 5]

Complexity Analysis:

Case| Time Complexity
Best case| O(n²) for this implementation
Average case| O(n²)
Worst case| O(n²)
Auxiliary space| O(1)

Key Takeaway:

Bubble Sort repeatedly compares adjacent elements and swaps them when necessary. It is easy to understand but inefficient for large datasets.

---

🛠️ Technologies and Tools

- Programming Language: Python
- Version Control: Git
- Code Repository: GitHub
- Learning Focus: DSA fundamentals, problem-solving, algorithm analysis

---

📈 Learning Summary

Through my first ten days of DSA learning, I have studied:

- [x] Introduction to Data Structures and Algorithms
- [x] Time complexity and Big O notation
- [x] Space complexity
- [x] Auxiliary space complexity
- [x] Algorithm analysis and complexity practice
- [x] Recursion fundamentals
- [x] Arrays and their operations
- [x] Linear Search
- [x] Binary Search
- [x] Sorting fundamentals
- [x] Bubble Sort

---

🎯 Upcoming Learning Goals

My next learning goals include:

- Selection Sort
- Insertion Sort
- Merge Sort and Quick Sort fundamentals
- More array-based coding problems
- Strings and common string manipulation problems
- Linked Lists
- Stacks and Queues
- Hashing and Dictionaries
- Trees and Graphs
- Searching and sorting problem practice
- Coding interview questions and placement preparation

Topics will be added as I learn and practise them.

---

💡 My Learning Philosophy

I believe that learning DSA is not just about memorizing algorithms. It is about understanding the underlying logic, choosing appropriate approaches, analysing complexity, and developing independent problem-solving skills.

I am documenting my progress consistently to track improvement, reinforce concepts, and build a practical foundation for future technical interviews.

One concept at a time. One problem at a time. Continuous improvement.

Thank you for visiting my DSA learning repository!
