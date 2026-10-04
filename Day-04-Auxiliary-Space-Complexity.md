Day 04: Auxiliary Space Complexity

1. Introduction

Auxiliary Space Complexity describes the extra memory an algorithm uses while executing, excluding the memory used to store the input under the usual convention.

It helps us understand how memory usage grows as the input size increases.

2. Space Complexity vs. Auxiliary Space Complexity

- Space Complexity: The total memory required by an algorithm, depending on the accounting convention.
- Auxiliary Space Complexity: The extra working memory used by an algorithm, excluding input storage under the usual convention.

Example: An algorithm that creates a new list to store results uses additional memory for that list.

3. Constant Auxiliary Space — O(1)

Constant auxiliary space means the extra memory usage stays constant as the input size grows.

Python Example

def add_numbers(a, b):
    result = a + b
    return result

print(add_numbers(5, 3))

Output:

8

Explanation:

- The function uses a fixed number of variables.
- It does not create a data structure that grows with the input size.
- Therefore, its auxiliary space complexity is O(1) under the usual analysis.

4. Linear Auxiliary Space — O(n)

Linear auxiliary space means the extra memory usage grows proportionally to the input size "n".

Python Example

def create_list(n):
    numbers = []

    for i in range(n):
        numbers.append(i)

    return numbers

print(create_list(4))

Output:

[0, 1, 2, 3]

Explanation:

- The function creates a new list.
- The list stores "n" elements.
- As "n" increases, the amount of memory required by the list increases.
- Therefore, its auxiliary space complexity is O(n).

5. Visual Understanding

O(1) — Constant Space

Input size:  10 → 100 → 1000
Extra space: Fixed amount

O(n) — Linear Space

Input size:  4    → 100  → 1000
List size:   4    → 100  → 1000

6. Comparison Table

Feature| O(1)| O(n)
Meaning| Constant extra memory| Linear extra memory
Memory growth| Stays constant| Grows with input size
Example| A fixed number of variables| A list containing n elements
Common use| Simple calculations| Storing results in a new list

7. Important DSA Concepts

- n: Represents the input size.
- O(1): Constant auxiliary space.
- O(n): Linear auxiliary space.
- O(n²): Quadratic space when the algorithm allocates a structure containing a number of elements proportional to n².
- Space complexity is about memory growth, not execution time.

Important: A nested loop does not automatically mean O(n²) auxiliary space. If it uses only a fixed number of extra variables, its auxiliary space can still be O(1).

8. Key Takeaways

1. Auxiliary space measures extra working memory.
2. O(1) means constant extra memory.
3. O(n) means extra memory grows linearly with input size.
4. Creating a new list of n elements typically requires O(n) auxiliary space.
5. Always examine the memory allocated by an algorithm instead of judging only by the number of code lines.

9. Practice Questions

Q1. What is the auxiliary space complexity of a function that uses a fixed number of variables?

Answer: O(1)

Q2. What is the auxiliary space complexity of creating a list containing n elements?

Answer: O(n)

Q3. Does a nested loop always require O(n²) auxiliary space?

Answer: No. Its auxiliary space can be O(1) if it uses only a fixed amount of extra memory.

10. Day 04 Summary

Today, I learned the meaning of auxiliary space complexity, the difference between space complexity and auxiliary space, and how to identify O(1) and O(n) auxiliary space using Python examples.

Next Goal: Continue learning DSA complexity analysis and strengthen problem-solving skills for technical interviews.
