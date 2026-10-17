Day 17: Two-Pointer Technique

📌 Overview

Today, I learned the Two-Pointer Technique, an important problem-solving technique in Data Structures and Algorithms (DSA).

It uses two pointers to traverse an array or string efficiently and solve problems with fewer unnecessary operations.

🎯 What Is the Two-Pointer Technique?

The Two-Pointer Technique uses two positions to process elements in a data structure.

A common approach is:

- Left pointer: starts at the beginning.
- Right pointer: starts at the end.
- Both pointers move toward each other according to the problem's requirements.

📝 Example 1: Reverse an Array

Input:

arr = [10, 20, 30, 40, 50]

Python Code:

arr = [10, 20, 30, 40, 50]

left = 0
right = len(arr) - 1

while left < right:
    arr[left], arr[right] = arr[right], arr[left]
    left += 1
    right -= 1

print(arr)

Output:

[50, 40, 30, 20, 10]

Explanation

1. Initialize the left pointer at index 0.
2. Initialize the right pointer at the last index.
3. Swap the values at both pointers.
4. Move the left pointer forward and the right pointer backward.
5. Stop when the pointers meet or cross.

📝 Example 2: Check Whether a String Is a Palindrome

A palindrome reads the same forward and backward.

Python Code:

text = "madam"

left = 0
right = len(text) - 1

while left < right:
    if text[left] != text[right]:
        print("Not a palindrome")
        break

    left += 1
    right -= 1
else:
    print("Palindrome")

Output:

Palindrome

Explanation

- Compare the first and last characters.
- If they differ, the string is not a palindrome.
- If they match, move both pointers toward the centre.
- If all pairs match, the string is a palindrome.

⏱️ Time and Space Complexity

Problem| Time Complexity| Auxiliary Space
Reverse an array| O(n)| O(1)
Check a palindrome| O(n)| O(1)

Here, "n" represents the number of elements or characters.

🚀 Applications

The Two-Pointer Technique can be used for:

- Reversing arrays and strings.
- Checking palindromes.
- Finding pairs with a target sum in sorted arrays.
- Removing duplicates from sorted arrays.
- Solving selected array and string problems.

💡 Key Takeaways

- Two pointers can reduce unnecessary operations.
- The pointers move according to the problem's logic.
- Some problems can be solved in linear time using this technique.
- The technique does not apply equally well to every array or string problem.

📚 Learning Progress

- Day: 17
- Topic: Two-Pointer Technique
- Concepts: Array reversal, palindrome checking, time complexity, and auxiliary space complexity.

Goal: Build strong DSA fundamentals and improve placement-level problem-solving skills.
