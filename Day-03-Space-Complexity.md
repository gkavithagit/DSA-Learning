Day 3: Space Complexity

What is Space Complexity?

Space complexity describes how the memory required by an algorithm grows as the input size increases.

Types of Complexity

1. Constant Space — O(1)

The extra memory remains constant regardless of input size.

Example:

total = 0

for num in numbers:
    total += num

2. Linear Space — O(n)

The extra memory grows proportionally to the input size.

Example:

squares = []

for num in numbers:
    squares.append(num * num)

Time Complexity vs Space Complexity

- Time complexity measures how the amount of work grows.
- Space complexity measures how memory usage grows.
- A loop can take O(n) time while using O(1) auxiliary space.

Key Takeaway

Space complexity helps us understand the memory trade-offs of an algorithm. Auxiliary space refers to extra memory used by the algorithm, excluding the input itself.

Progress

- Day 1: Introduction to DSA
- Day 2: Big O Notation and Time Complexity
- Day 3: Space Complexity

Next: Arrays and how to solve array problems logically.
