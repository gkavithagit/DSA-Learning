Day 18: Binary Search — First and Last Occurrence

📌 Today's Learning

Today, I learned how to find the first and last occurrences of a target element in a sorted array using Binary Search.

🎯 Concepts Covered

- Finding the first occurrence of an element.
- Finding the last occurrence of an element.
- Understanding how Binary Search handles duplicate elements.
- Using the left and right search boundaries effectively.
- Returning "-1" when the target element is not found.
- Understanding time and auxiliary space complexity.

💡 Example

Input:

arr = [2, 4, 4, 4, 4, 7, 9]
target = 4

Output:

First occurrence index: 1
Last occurrence index: 4

⚙️ Approach

First Occurrence:

1. Apply Binary Search to the sorted array.
2. When the target is found, store its index.
3. Continue searching in the left half.
4. Return the earliest matching index.

Last Occurrence:

1. Apply Binary Search to the sorted array.
2. When the target is found, store its index.
3. Continue searching in the right half.
4. Return the latest matching index.

If the target does not exist, return "-1".

⏱️ Time and Space Complexity

- Time Complexity: O(log n) for each search.
- Auxiliary Space Complexity: O(1) for the iterative approach.

🧠 Key Takeaway

Binary Search can do more than find an element. By adjusting the search direction after finding a match, we can identify the first and last occurrences efficiently, even when duplicate elements exist.
Next Goal: Practise more Binary Search problems and improve my problem-solving skills.
