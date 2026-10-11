📅 Day 11: Binary Search

🎯 Learning Objective

Understand Binary Search, how it works, why sorted data is required, and how its time complexity compares with Linear Search.

📚 Concepts Learned

1. What is Binary Search?

Binary Search is a searching algorithm that finds a target element by repeatedly dividing a sorted search space into two halves.

Instead of checking every element individually, it compares the target with the middle element and eliminates half of the remaining search space.

2. How Binary Search Works

Example array:

"[10, 20, 30, 40, 50, 60, 70]"

Target: "60"

- Step 1: Check the middle element, "40".
- Step 2: Since "60 > 40", eliminate the left half.
- Step 3: Check the middle of the remaining search space, "60".
- Step 4: Target found!

3. Important Requirement

The standard Binary Search algorithm requires sorted data.

Example of sorted data:
"[10, 20, 30, 40, 50]"

Example of unsorted data:
"[30, 10, 50, 20, 40]"

Standard Binary Search cannot be directly applied to the unsorted array.

4. Time Complexity

Case| Time Complexity
Best Case| O(1)
Average Case| O(log n)
Worst Case| O(log n)

5. Space Complexity

For an iterative Binary Search implementation, auxiliary space complexity is O(1), because it uses a constant amount of additional memory.

⚖️ Linear Search vs Binary Search

Feature| Linear Search| Binary Search
Approach| Checks elements one by one| Repeatedly halves the search space
Sorted data required| No| Yes, for the standard approach
Worst-case time| O(n)| O(log n)
Iterative auxiliary space| O(1)| O(1)

💡 Key Takeaways

- Binary Search is efficient for searching sorted arrays.
- Each comparison eliminates approximately half of the remaining search space.
- Its worst-case time complexity is O(log n).
- Iterative Binary Search uses O(1) auxiliary space.
- Choosing the right algorithm can significantly improve program efficiency.

✅ Day 11 Progress

- [x] Understood Binary Search fundamentals.
- [x] Learned the importance of sorted arrays.
- [x] Compared Linear Search and Binary Search.
- [x] Reviewed time and auxiliary space complexity.
- [x] Completed a 5-question knowledge assessment with a score of 5/5.
