🚀 Data Structures and Algorithms (DSA) — My Learning Journey

📌 About This Repository

Welcome to my Data Structures and Algorithms (DSA) learning repository!

This repository documents my daily progress in learning DSA using Python. My goal is to develop strong problem-solving skills, understand algorithmic thinking, write efficient code, and prepare for technical interviews and future software development opportunities.

Instead of memorizing solutions, I focus on understanding the logic behind each problem, practising implementation, analysing time and space complexity, and improving my ability to solve problems independently.

Learning Progress: Day 1 – Day 25
Programming Language: Python 🐍
Focus Areas: Problem-Solving, Arrays, Searching Algorithms, Strings, Hash Maps, and Algorithm Analysis.

---

🎯 Learning Objectives

- Build a strong foundation in Data Structures and Algorithms.
- Understand how to analyse algorithm efficiency.
- Learn to solve problems using Python.
- Improve logical thinking and computational problem-solving.
- Understand the time and space complexity of algorithms.
- Develop the ability to choose efficient solutions.
- Maintain a consistent daily coding practice routine.
- Prepare for coding interviews and future technical opportunities.

---

📚 DSA Learning Progress

🔹 Day 1: Introduction to DSA

Topics Covered

- Introduction to Data Structures and Algorithms.
- Understanding Python lists as a way to store collections of elements.
- Array/list indexing and the concept of zero-based indexing.
- Accessing and traversing elements.
- Finding the largest and smallest elements in a list.
- Introduction to linear search.
- Basic list operations, including adding and removing elements.
- Checking whether an element exists in a list.
- Counting occurrences of elements.

Key Learnings

Learned how to traverse a list, compare elements, update variables, and use basic searching techniques to solve simple problems.

Also developed an initial understanding of how the number of elements affects an algorithm's execution time.

---

🔹 Days 2–5: Building Programming Logic and DSA Fundamentals

Focused on strengthening the basic concepts needed to solve DSA problems.

Learning Focus

- Understanding problem statements.
- Breaking problems into smaller steps.
- Using variables and conditional logic.
- Working with loops and collections.
- Practising array/list traversal.
- Developing step-by-step problem-solving logic.

Key Learnings

Developed a foundation for translating problem statements into logical steps and implementing solutions in Python.

Note: This section summarises the foundational learning phase rather than assigning specific unverified topics to individual days.

---

🔹 Days 6–9: Arrays and Problem-Solving Practice

Learning Focus

- Working with arrays and Python lists.
- Accessing elements through indices.
- Traversing collections.
- Finding maximum and minimum values.
- Searching for elements.
- Counting occurrences.
- Understanding basic list methods.
- Analysing simple solutions.

Python List Operations

Practised or reviewed commonly used list operations, including:

- "append()" — Add an element to the end.
- "insert()" — Insert an element at a specified position.
- "extend()" — Add multiple elements.
- "remove()" — Remove an element by value.
- "pop()" — Remove and return an element.
- "clear()" — Remove all elements.
- "index()" — Find the index of an element.
- "count()" — Count occurrences.
- "sort()" — Sort a list in place.
- "reverse()" — Reverse a list in place.
- "sorted()" — Return a sorted version of an iterable.

Key Learnings

Strengthened understanding of list manipulation, element searching, and the importance of choosing appropriate operations for a problem.

---

🔹 Days 10–13: Searching Algorithms and Binary Search

Studied searching algorithms, with particular attention to understanding and practising binary search.

1. Linear Search

Linear search examines elements sequentially until the target is found or the collection ends.

Example:

def linear_search(arr, target):
    for i, num in enumerate(arr):
        if num == target:
            return i
    return -1

Complexity:

- Best-case time: O(1)
- Worst-case time: O(n)
- Auxiliary space: O(1)

2. Binary Search

Binary search efficiently searches a sorted array by repeatedly dividing the search interval into two halves.

Important Concepts

- "low": The lower boundary of the search interval.
- "high": The upper boundary of the search interval.
- "mid": The middle index of the interval.
- Comparing the middle element with the target.
- Updating the search boundaries.
- Repeating until the target is found or the interval becomes empty.

Python Implementation

def binary_search(arr, target):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = low + (high - low) // 2

        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1

    return -1

Complexity

- Best-case time: O(1)
- Worst-case time: O(log n)
- Auxiliary space: O(1)

Important: Standard binary search requires the input to be sorted.

Linear Search vs. Binary Search

Feature| Linear Search| Binary Search
Input requirement| Works on sorted or unsorted arrays| Requires sorted input
Search method| Checks elements sequentially| Repeatedly halves the search interval
Worst-case time| O(n)| O(log n)
Auxiliary space| O(1) for the iterative version| O(1) for the iterative version

Key Learnings

Understood how binary search reduces the search space and why it is generally more efficient than linear search on large, sorted arrays.

---

🔹 Days 14–20: Binary Search Practice and Occurrence Problems

Focused on strengthening binary search through repeated practice, revision, and problem-solving exercises.

Learning Focus

- Reviewing the binary search algorithm.
- Understanding search boundaries.
- Updating "low", "high", and "mid" correctly.
- Tracing the algorithm step by step.
- Identifying common binary search mistakes.
- Solving variations of binary search.
- Finding the first occurrence of a target.
- Finding the last occurrence of a target.
- Understanding how duplicate elements affect search results.

First and Last Occurrence

Consider the sorted array:

arr = [1, 2, 2, 2, 3, 4, 5]
target = 2

The first occurrence of "2" is at index "1".

The last occurrence of "2" is at index "3".

A standard binary search may return any matching occurrence. To find the first or last occurrence, the algorithm must continue searching after finding a match.

General Approach

First occurrence:

- When the target is found, record its index.
- Continue searching the left half.

Last occurrence:

- When the target is found, record its index.
- Continue searching the right half.

Complexity

- Time: O(log n) for each binary-search-based occurrence search.
- Auxiliary space: O(1) for an iterative implementation.

Key Learnings

Improved the ability to trace binary search, manage search boundaries, and modify a standard algorithm to solve related problems.

Repeated practice also helped reinforce the difference between finding an element and finding its first or last position.

---

🔹 Days 21–22: Binary Search Revision and Continued Practice

Learning Focus

- Revising binary search concepts.
- Practising first and last occurrence problems.
- Strengthening understanding of sorted arrays.
- Applying binary search to target-search problems.
- Improving accuracy through quizzes and algorithm tracing.

Key Learnings

Reinforced the importance of correctly updating search boundaries and understanding how the algorithm reduces the remaining search space.

Focused on improving problem-solving accuracy rather than simply memorising code.

---

🔹 Day 23: Palindrome Problems

Studied palindrome problems involving strings.

What Is a Palindrome?

A palindrome is a sequence that reads the same forward and backward.

Examples:

- "madam" — Palindrome.
- "level" — Palindrome.
- "hello" — Not a palindrome.

Basic Python Implementation

def is_palindrome(s):
    return s == s[::-1]

How It Works

- "s[::-1]" creates a reversed version of the string.
- The original string is compared with its reversed version.
- If both are equal, the string is a palindrome.

Complexity

For a string of length n:

- Time: O(n).
- Auxiliary space: O(n) for the reversed string created by slicing.

Key Learnings

Developed an understanding of palindrome checking, string reversal, equality comparison, and basic string-based problem-solving.

---

🔹 Day 24: Anagram Problems

Studied anagram problems and the relationship between character frequencies in strings.

What Is an Anagram?

Two strings are anagrams if they contain exactly the same characters with the same frequencies, regardless of their order.

Example:

String 1: listen
String 2: silent
Result: True

Both strings contain the same characters with identical frequencies.

Basic Python Implementation

from collections import Counter

def is_anagram(s1, s2):
    return Counter(s1) == Counter(s2)

How It Works

- "Counter()" counts the occurrences of each character.
- Both character-frequency mappings are compared.
- If the frequencies match, the strings are anagrams.

Complexity

For two strings of lengths n and m:

- Time: O(n + m) on average.
- Auxiliary space: O(n + m) in the general case.

Key Learnings

Learned the importance of character frequencies, string comparison, and using suitable data structures to simplify problems.

---

🔹 Day 25: Two Sum Problem Using a Hash Map

Studied the Two Sum problem, which demonstrates how a Hash Map can improve the efficiency of array-based problem-solving.

Problem Statement

Given an array of integers and a target value, find the indices of two distinct elements whose sum equals the target.

Example

arr = [2, 7, 11, 15]
target = 9

Output:

[0, 1]

Because:

arr[0] + arr[1] = 2 + 7 = 9

Approach

1. Create an empty dictionary.

2. Traverse the array while tracking each element's index.

3. Calculate the required complement:
   
   "complement = target - current_number"

4. Check whether the complement already exists in the dictionary.

5. If it exists, return the stored index and the current index.

6. Otherwise, store the current number and its index.

7. If no valid pair exists, return an empty list.

Python Implementation

def two_sum(arr, target):
    seen = {}

    for i, num in enumerate(arr):
        needed = target - num

        if needed in seen:
            return [seen[needed], i]

        seen[num] = i

    return []


arr = [2, 7, 11, 15]
target = 9

print(two_sum(arr, target))

Output:

[0, 1]

Complexity Analysis

- Average-case time complexity: O(n).
- Auxiliary space complexity: O(n) in the worst case.

The dictionary allows the algorithm to check for a previously visited complement without searching the entire array again.

Key Learnings

- Understanding the Two Sum problem.
- Using a Python dictionary as a Hash Map.
- Applying the complement technique.
- Using "enumerate()" to access indices and values.
- Understanding the time-space trade-off.
- Comparing a Hash Map solution with a brute-force approach.

A brute-force solution checks every possible pair and takes O(n²) time in the worst case. The Hash Map approach improves the average-case running time to O(n).

---

🧠 Core Concepts Learned

Throughout this learning journey, I have been developing my understanding of the following concepts.

1. Data Structures

- Python lists as array-like collections.
- Indexing and traversal.
- Basic dictionary operations and Hash Map usage.

2. Searching Algorithms

- Linear search.
- Binary search.
- First occurrence of a target.
- Last occurrence of a target.

3. String Problems

- Palindrome checking.
- String reversal.
- Anagram checking.
- Character-frequency comparison.

4. Algorithmic Techniques

- Sequential traversal.
- Divide-and-conquer searching.
- Search-space reduction.
- Complement-based searching.
- Hash Map lookups.

5. Complexity Analysis

- Understanding O(1), O(log n), O(n), and O(n²).
- Analysing time complexity.
- Understanding auxiliary space complexity.
- Comparing straightforward solutions with more efficient approaches.

6. Python Programming Skills

- Lists and list methods.
- Loops and conditional statements.
- Functions and return values.
- String slicing.
- Dictionaries.
- "enumerate()".
- "collections.Counter".

---

📊 Time Complexity Reference

Complexity| Meaning| Example
O(1)| Constant time| Accessing an element by index
O(log n)| Logarithmic time| Binary search
O(n)| Linear time| Linear search in the worst case
O(n²)| Quadratic time| Checking every possible pair using nested loops

Understanding complexity helps me evaluate whether a solution is suitable for larger inputs.

---

💡 My Problem-Solving Approach

My approach to solving DSA problems is becoming more structured:

1. Understand: Identify the input, expected output, and constraints.
2. Plan: Develop a logical approach before writing code.
3. Implement: Convert the logic into Python.
4. Dry Run: Trace the algorithm with an example.
5. Test: Check normal cases and important edge cases.
6. Analyse: Evaluate time and auxiliary space complexity.
7. Improve: Look for a more efficient solution when appropriate.

This process helps me focus on understanding why an algorithm works rather than memorising code.

---

🎯 Future Learning Goals

My next goal is to continue developing my DSA skills through consistent practice.

Planned areas of study include:

- More array and string problems.
- Hash Map and frequency-counting problems.
- Two-pointer techniques.
- Sliding-window techniques.
- Prefix sums.
- Sorting algorithms.
- Recursion and backtracking fundamentals.
- Stack and queue data structures.
- Linked lists.
- More interview-style coding problems.

These are future learning goals, not claims that every topic has already been completed.

---

📈 Progress Summary

Milestone| Learning Area| Status
Day 1| DSA fundamentals and introductory array operations| Completed
Days 2–9| Programming logic, arrays, and problem-solving practice| Learning phase completed
Days 10–13| Searching algorithms and binary search fundamentals| Completed
Days 14–22| Binary search practice and occurrence problems| Practised
Day 23| Palindrome problems| Completed
Day 24| Anagram problems| Completed
Day 25| Two Sum using a Hash Map| Studied and practised

---

🚀 Conclusion

My first 25 days of DSA learning have helped me build a foundation in array operations, searching algorithms, binary search, string problems, and introductory Hash Map techniques.

I am focusing on consistent practice, logical thinking, and understanding algorithm efficiency.

My objective is not just to write code that works, but to understand why it works, analyse its performance, and gradually solve more challenging problems independently.

25 days of learning. One step closer to becoming a better problem solver. 💻

---

⭐ This repository represents my ongoing DSA learning journey. I will continue updating it as I learn new concepts, practise more problems, and improve my solutions.
