Day 28: Character Frequency Counting in Python

📌 Overview

Today, I learned how to count the frequency of each character in a string using Python dictionaries. This technique is useful in string manipulation, coding interviews, and various problem-solving tasks.

🎯 Learning Objectives

- Understand character frequency counting.
- Use Python dictionaries to store character counts.
- Traverse strings using a "for" loop.
- Update dictionary values using conditional statements.
- Understand the time and space complexity of frequency counting.
- Explore Python's "collections.Counter" utility.

💡 Approach 1: Using a Dictionary

Problem

Given a string, count how many times each character appears.

Python Code

word = "banana"
frequency = {}

for char in word:
    if char in frequency:
        frequency[char] += 1
    else:
        frequency[char] = 1

print(frequency)

Output

{'b': 1, 'a': 3, 'n': 2}

Explanation

1. Initialize an empty dictionary.
2. Traverse the string character by character.
3. Check whether each character already exists in the dictionary.
4. If it exists, increment its count.
5. Otherwise, add the character with an initial count of 1.
6. Print the completed frequency dictionary.

⚡ Approach 2: Using Dictionary "get()"

word = "banana"
frequency = {}

for char in word:
    frequency[char] = frequency.get(char, 0) + 1

print(frequency)

The "get()" method returns the existing count if the character is present. Otherwise, it returns the default value of "0". Adding "1" updates the character's frequency.

This approach reduces the number of lines while preserving the same counting logic.

🐍 Approach 3: Using "collections.Counter"

from collections import Counter

word = "banana"
frequency = Counter(word)

print(frequency)

Output

Counter({'a': 3, 'n': 2, 'b': 1})

"Counter" is a Python utility designed to count the occurrences of elements in an iterable, including characters in strings.

⏱️ Complexity Analysis

For the dictionary-based solution:

- Time Complexity: O(n) on average, where "n" is the length of the string.
- Auxiliary Space Complexity: O(k), where "k" is the number of distinct characters stored in the dictionary.

🧪 Practice Examples

Example 1

Input:

apple

Output:

a: 1
p: 2
l: 1
e: 1

Example 2

Input:

level

Output:

l: 2
e: 2
v: 1

🌍 Real-World Applications

- Detecting repeated characters in strings.
- Checking whether two strings are anagrams.
- Analyzing character distributions in text.
- Solving string-based coding interview problems.
- Counting words or other elements using similar dictionary techniques.

📚 Key Takeaways

- Dictionaries store data as key-value pairs.
- Each distinct character becomes a dictionary key.
- Dictionary values represent character frequencies.
- The "get()" method provides a concise way to update counts.
- "Counter" offers a convenient built-in alternative.
- Frequency counting is an important foundation for string-based DSA problems.

✅ Progress

Day 28 completed: Character Frequency Counting in Python.
