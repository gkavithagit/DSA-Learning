📚 DSA Day 7 — Arrays & Linked Lists

Today I learned the fundamentals of Arrays and Linked Lists, with a focus on understanding how different operations affect time and space complexity.

🔹 Topics Covered

1. Arrays

- Understanding arrays and indexing
- Zero-based indexing
- Accessing elements using an index
- Traversing an array
- Searching elements
- Insertion and deletion
- Understanding why elements may need to be shifted

2. Array Time Complexity

Operation| Time Complexity
Access by index| O(1)
Traversal| O(n)
Linear Search| O(n)
Insert at beginning/middle| O(n)
Delete at beginning/middle| O(n)
Append at end| O(1) amortized

3. Why Insertion and Deletion Can Be O(n)

When an element is inserted or deleted from the beginning or middle of an array, other elements may need to shift.

Insertion:

[10] [20] [30] [40]

Insert 25

[10] [20] [25] [30] [40]
                  ← elements shift

Deletion:

[10] [20] [30] [40]

Delete 20

[10] [30] [40]
      ← elements shift

This shifting is why these operations can take O(n) time.

🔗 4. Linked Lists

I learned why Linked Lists are used as an alternative data structure.

A Linked List consists of nodes containing:

[Data | Next]

Example:

10 → 20 → 30 → 40 → NULL

Unlike an array, nodes do not need to be stored next to each other. Each node keeps a reference to the next node.

Array vs Linked List

Operation| Array| Linked List
Access by index| O(1)| O(n)
Search| O(n)| O(n)
Insert at beginning| O(n)| O(1)*
Delete at beginning| O(n)| O(1)*
Access random element| Fast| Slow

"*" Assuming the required node/reference is already available.

💻 5. Problem Solving Practice

Problem: Find the Largest Element

Given:

arr = [7, 23, 4, 91, 18, 36]

I solved it using a running maximum approach:

largest = arr[0]

for num in arr:
    if num > largest:
        largest = num

print(largest)

Output:

91

Complexity

- Time Complexity: O(n)
- Space Complexity: O(1)

The algorithm scans the array once and uses only one additional variable.

🧠 Key Learning

Today's main takeaway was understanding that choosing a data structure involves a trade-off.

- Arrays provide fast random access.
- Linked Lists can make insertion and deletion easier when the required node/reference is known.
- The right data structure depends on the problem requirements.

🚀 Day 7 Progress

Completed:

- Arrays
- Array indexing
- Traversal
- Searching
- Insertion & deletion
- Array complexity analysis
- Linked Lists introduction
- Array vs Linked List comparison
- Largest element problem

Continuing to build my DSA foundation step by step with a focus on problem-solving, complexity analysis, and placement preparation.
