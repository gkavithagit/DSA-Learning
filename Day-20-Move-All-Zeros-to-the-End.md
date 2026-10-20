DSA Day 20: Move All Zeros to the End

📌 Topic

Array Problem Solving — Move All Zeros to the End

🎯 Learning Objective

Today, I learned how to solve an array problem by moving all zeros to the end of an array while maintaining the relative order of non-zero elements.

🧠 Problem Statement

Given an array containing zeros and non-zero integers, move all zeros to the end without changing the relative order of the non-zero elements.

Example

Input:

arr = [0, 1, 0, 4, 5]

Output:

[1, 4, 5, 0, 0]

📚 Concepts Learned

- Array manipulation
- Conditional statements
- Iteration using loops
- Two-pointer technique
- In-place array modification
- Time and space complexity analysis

💡 Approach 1: Simple Method

Separate the non-zero elements and zeros into two lists, then combine them.

arr = [0, 1, 0, 4, 5]

non_zero = [x for x in arr if x != 0]
zeros = [x for x in arr if x == 0]

result = non_zero + zeros

print(result)

Output:

[1, 4, 5, 0, 0]

Time Complexity: O(n)
Auxiliary Space Complexity: O(n)

🚀 Approach 2: Two-Pointer Technique

Move non-zero elements to the beginning of the original array, then fill the remaining positions with zeros.

arr = [0, 1, 0, 4, 5]

position = 0

for i in range(len(arr)):
    if arr[i] != 0:
        arr[position] = arr[i]
        position += 1

while position < len(arr):
    arr[position] = 0
    position += 1

print(arr)

Output:

[1, 4, 5, 0, 0]

How the Logic Works

1. Initialize "position = 0" to track where the next non-zero element should be placed.
2. Traverse the array and identify non-zero elements.
3. Place each non-zero element at the current "position".
4. Increment "position" after each placement.
5. Fill all remaining positions with zeros.

⏱️ Complexity Analysis

Approach| Time Complexity| Auxiliary Space
Simple Method| O(n)| O(n)
Two-Pointer Method| O(n)| O(1)

🔑 Key Takeaways

- Two pointers can help solve array manipulation problems efficiently.
- Preserving the relative order of elements is important in this problem.
- In-place modification can reduce auxiliary space usage.
- Understanding the logic is more important than memorizing the code.

🎯 Practice Challenge

Input:

arr = [0, 7, 0, 2, 9, 0, 3]

Expected Output:

[7, 2, 9, 3, 0, 0, 0]

📈 Daily Progress

Day 20 completed successfully!

I practiced array manipulation, explored two approaches, and learned how the two-pointer technique can optimize space complexity.

Next Goal: Continue practicing DSA problems and strengthen problem-solving skills for coding interviews and placements.
