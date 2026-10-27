Day 27: Find All Occurrences of a Character in a String

📌 Problem Statement

Given a string and a target character, find and return all the indices where the target character occurs in the string.

The indices must follow Python's zero-based indexing.

🎯 Objectives

- Understand string traversal.
- Identify every occurrence of a target character.
- Practise zero-based indexing.
- Use Python's "enumerate()" function.
- Analyse time and space complexity.

💻 Example

Input:

text = "programming"
target = "g"

Output:

[3, 10]

Explanation:

The character "'g'" appears at indices "3" and "10" in the string ""programming"".

🛠️ Approach 1: Using a For Loop

def find_occurrences(text, target):
    positions = []

    for i in range(len(text)):
        if text[i] == target:
            positions.append(i)

    return positions


print(find_occurrences("programming", "g"))

Output:

[3, 10]

Algorithm:

1. Create an empty list to store the indices.
2. Traverse the string using a loop.
3. Compare each character with the target character.
4. If they match, append the current index to the list.
5. Return the list of indices.

⚡ Approach 2: Using "enumerate()"

def find_occurrences(text, target):
    return [
        i for i, char in enumerate(text)
        if char == target
    ]


print(find_occurrences("banana", "a"))

Output:

[1, 3, 5]

Explanation:

The "enumerate()" function provides both the index and the character during iteration. A list comprehension collects the indices where the character matches the target.

⏱️ Complexity Analysis

Let:

- "n" = length of the input string.
- "k" = number of occurrences of the target character.

Complexity| Analysis
Time Complexity| O(n)
Auxiliary Space Complexity| O(k)

The algorithm checks every character once. The output list stores the matching indices.

🧠 Key Learnings

- Strings can be traversed character by character.
- Python indexing starts at zero.
- A loop can be used to find multiple matches.
- "enumerate()" provides both an index and its corresponding element.
- Both approaches have O(n) time complexity.

🚀 Day 27 Outcome

Practised string traversal, character searching, index collection, and complexity analysis using Python.

Next Goal: Continue solving new DSA problems and strengthen problem-solving skills for technical interviews and campus placements.
