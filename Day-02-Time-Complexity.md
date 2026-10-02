Day 02 — Time Complexity and Big O Notation

Overview

On Day 2 of my Data Structures and Algorithms (DSA) learning journey, I studied Time Complexity and Big O Notation to understand how an algorithm's efficiency changes as the input size grows.

The focus was on understanding the logic behind algorithm analysis and identifying common time complexities using Python examples.

Topics Covered

- What is Time Complexity?
- Introduction to Big O Notation
- Constant Time — "O(1)"
- Linear Time — "O(n)"
- Quadratic Time — "O(n²)"
- Understanding sequential loops and nested loops
- Analyzing the number of operations performed by an algorithm

1. What Is Time Complexity?

Time complexity describes how the amount of work an algorithm performs grows as the input size increases.

It helps us analyze and compare algorithms without depending on a specific computer's execution time.

2. Understanding Big O Notation

Big O notation describes the growth rate of an algorithm's resource usage as its input size increases.

Common Time Complexities

Complexity| Name| Example
"O(1)"| Constant| Accessing an element by index
"O(log n)"| Logarithmic| Binary search on sorted data
"O(n)"| Linear| Traversing a list
"O(n log n)"| Linearithmic| Merge sort
"O(n²)"| Quadratic| Two nested loops over the same list

3. Python Examples

Example 1: Constant Time — O(1)

numbers = [10, 20, 30, 40, 50]
print(numbers[0])

Explanation: Accessing a list element using a known index takes constant time under the usual array-based list model.

Time Complexity: "O(1)"

Example 2: Linear Time — O(n)

numbers = [10, 20, 30, 40, 50]

for number in numbers:
    print(number)

Explanation: The loop visits every element once. The amount of work grows with the number of elements.

Time Complexity: "O(n)"

Example 3: Quadratic Time — O(n²)

numbers = [10, 20, 30]

for i in numbers:
    for j in numbers:
        print(i, j)

Explanation: For every element in the outer loop, the inner loop visits every element again.

For "n" elements, the inner statement executes "n × n" times.

Time Complexity: "O(n²)"

Example 4: Two Sequential Loops — O(n)

numbers = [10, 20, 30, 40, 50]

for number in numbers:
    print(number)

for number in numbers:
    print(number)

Explanation: Both loops run one after another. Their combined work is "n + n = 2n".

Big O ignores constant factors, so the time complexity is "O(n)".

4. Practice and Learning Outcomes

During today's practice, I analyzed four questions involving list access, a single loop, nested loops, and operation counting.

- Identified constant-time list access.
- Recognized linear iteration through a list.
- Understood how nested loops produce quadratic growth.
- Calculated the operations in nested loops: "10 × 10 = 100".
- Learned that two sequential linear loops are "O(n)", not "O(n²)".

Key Takeaway

Understanding Big O notation is an important foundation for analyzing algorithm efficiency. I am learning to focus on how the number of operations grows rather than simply whether a Python program produces the correct output.

Learning Progress

- Day 01: Introduction to DSA
- Day 02: Time Complexity and Big O Notation

Next: Continue building DSA fundamentals and practice analyzing algorithms with Python.
