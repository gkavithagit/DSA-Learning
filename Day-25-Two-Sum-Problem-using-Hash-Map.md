Day 25: Two Sum Problem Using Hash Map

📌 Overview

Today, I learned how to solve the Two Sum problem using a Hash Map (Python dictionary). This approach improves efficiency by storing previously visited numbers and their indices.

🎯 Problem Statement

Given an array of integers and a target value, find the indices of two distinct elements whose sum equals the target.

💡 Approach

1. Create an empty dictionary named "seen".
2. Traverse the array using "enumerate()" to obtain each element and its index.
3. Calculate the complement using "target - num".
4. Check whether the complement exists in the dictionary.
5. If it exists, return the stored index of the complement and the current index.
6. Otherwise, store the current number and its index in the dictionary.
7. If no valid pair is found, return an empty list.

💻 Python Implementation

def two_sum(arr, target):
    seen = {}

    for i, num in enumerate(arr):
        needed = target - num

        if needed in seen:
            return [seen[needed], i]

        seen[num] = i

    return []


arr = [2, 7, 11, 15]
target = 9

print(two_sum(arr, target))

Output:

[0, 1]

🔍 Example Explanation

Given:

- Array: "[2, 7, 11, 15]"
- Target: "9"

The algorithm processes the array as follows:

- At index 0, the number is "2". Its complement is "7". Since "7" is not in the dictionary, store "2" with index "0".
- At index 1, the number is "7". Its complement is "2". The dictionary already contains "2" at index "0".
- Return "[0, 1]" because "2 + 7 = 9".

⏱️ Complexity Analysis

- Time Complexity: O(n) average case, where n is the number of elements in the array.
- Auxiliary Space Complexity: O(n) in the worst case because the dictionary may store nearly all elements.

📚 Key Learnings

- Understanding the Two Sum problem.
- Using Python dictionaries as Hash Maps.
- Applying the complement technique.
- Using "enumerate()" to access elements and indices.
- Improving time complexity from O(n²) with brute force to O(n) average case.
- Understanding the time-space trade-off in algorithm design.

✅ Day 25 Achievement

Learned and implemented the Hash Map approach to the Two Sum problem and reviewed its time and space complexity.

Next Goal: Practise variations of Two Sum and learn when Hash Maps are useful for solving array and searching problems.
