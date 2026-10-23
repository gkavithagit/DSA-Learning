📅 Day 23: Palindrome Problems — Two-Pointer Technique

📌 Overview

On Day 23 of my Data Structures and Algorithms (DSA) learning journey, I studied palindrome problems and learned how to check whether a string reads the same forward and backward using Python.

I explored two approaches: string reversal and the Two-Pointer Technique. I also analyzed their time and space complexities.

📚 Concepts Covered

- Palindrome: A string that remains the same when reversed.
- String Reversal: Using Python slicing to reverse a string.
- Two-Pointer Technique: Comparing characters from opposite ends of a string.
- Conditional Logic: Returning "True" or "False" based on character comparisons.
- Time Complexity: Understanding why palindrome checking takes O(n) time in the worst case.
- Space Complexity: Understanding how the two-pointer approach avoids creating an additional reversed string.

💻 Python Implementation

def is_palindrome(s):
    left = 0
    right = len(s) - 1

    while left < right:
        if s[left] != s[right]:
            return False

        left += 1
        right -= 1

    return True


print(is_palindrome("madam"))   # True
print(is_palindrome("racecar")) # True
print(is_palindrome("hello"))   # False
print(is_palindrome("radar"))   # True

🔍 How the Algorithm Works

1. Initialize "left" to the first index and "right" to the last index.
2. Compare the characters at both positions.
3. If the characters differ, return "False".
4. If they match, move "left" one position forward and "right" one position backward.
5. Repeat until the pointers meet or cross.
6. If all corresponding characters match, return "True".

⏱️ Complexity Analysis

Complexity| Value| Explanation
Time Complexity| O(n)| In the worst case, the algorithm compares approximately half the characters, which is O(n).
Auxiliary Space Complexity| O(1)| Only two pointer variables are used, excluding the input string.

📝 Learning Outcome

By completing Day 23, I strengthened my understanding of string manipulation and learned to apply the Two-Pointer Technique to palindrome problems.

I also practiced analyzing algorithm efficiency and understood how to solve the same problem using different approaches.

Key Takeaway: Choosing an appropriate algorithm can improve space efficiency without increasing time complexity.
