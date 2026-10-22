Day 22 Character Frequency in Strings

📌 Topic

Character Frequency Counting Using Python Dictionaries

Today, I learned how to count the frequency of each character in a string using Python dictionaries. This is an important problem-solving technique used in Data Structures and Algorithms (DSA) and coding interviews.

🎯 Learning Objectives

- Understand character frequency counting.
- Use Python dictionaries to store character counts.
- Apply conditional statements and loops to solve string problems.
- Understand how to find repeated and non-repeating characters.
- Analyze the time and space complexity of the solution.

🧠 Concept Explanation

Character frequency counting determines how many times each character appears in a given string.

For example:

Input:

text = "banana"

Output:

{'b': 1, 'a': 3, 'n': 2}

A dictionary stores each unique character as a key and its frequency as the corresponding value.

💻 Python Implementation

text = "banana"
frequency = {}

for char in text:
    if char in frequency:
        frequency[char] += 1
    else:
        frequency[char] = 1

print(frequency)

Output:

{'b': 1, 'a': 3, 'n': 2}

⚙️ Algorithm

1. Initialize an empty dictionary.
2. Traverse the string character by character.
3. Check whether the current character exists in the dictionary.
4. If it exists, increment its frequency by one.
5. Otherwise, add the character with a frequency of one.
6. Display the resulting dictionary.

⏱️ Complexity Analysis

- Time Complexity: O(n), where n is the length of the string, assuming average O(1) dictionary operations.
- Auxiliary Space Complexity: O(k), where k is the number of distinct characters.

🚀 Practice Problem: First Non-Repeating Character

Given a string, find the first character that occurs exactly once.

Example:

Input:

text = "aabbcde"

Output:

c

Approach:

1. Count the frequency of every character.
2. Traverse the original string again.
3. Return the first character whose frequency equals one.
4. If no such character exists, report that no non-repeating character is present.

📚 Key Takeaways

- Dictionaries are useful for frequency-counting problems.
- A character's frequency can be updated using "frequency[char] += 1".
- Two traversals can solve many string-frequency problems efficiently.
- Understanding the logic is more important than memorizing code.

📈 Progress

DSA Learning Challenge — Day 22 Completed

Continuing to build strong foundations in Python, DSA, algorithmic thinking, and placement-oriented problem-solving.
