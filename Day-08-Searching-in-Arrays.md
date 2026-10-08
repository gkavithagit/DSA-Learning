DSA Day 8 — Searching in Arrays 🔎

Today I learned the fundamentals of Searching in Arrays, with a focus on Linear Search.

📚 Topics Covered

1. What is Searching?

Searching is the process of finding a specific target element inside a data structure such as an array.

2. Linear Search

Linear Search checks elements one by one from the beginning of the array until:

- The target element is found, or
- The entire array has been checked.

Example:

Array:  [10, 25, 7, 91, 43]
Target: 91

10 ❌ → 25 ❌ → 7 ❌ → 91 ✅

3. Time Complexity

Case| Complexity| Explanation
Best Case| O(1)| Target is the first element
Average Case| O(n)| Target may be somewhere in the array
Worst Case| O(n)| Target is last or not present

4. Space Complexity

Auxiliary Space: O(1)

Linear Search only uses a small number of additional variables and does not require another array.

💻 Python Implementation

arr = [10, 25, 7, 91, 43]
target = 91

for i in range(len(arr)):
    if arr[i] == target:
        print("Found at index", i)
        break

Output:

Found at index 3

🧠 Key Learning

The important lesson from today was not simply memorizing that Linear Search is "O(n)".

I learned why it becomes "O(n)" in the worst case: the algorithm may need to inspect every element.

Complexity Summary

Linear Search

Best Case    → O(1)
Average Case → O(n)
Worst Case   → O(n)
Space        → O(1)



#DSA #LinearSearch #Arrays #Python #DataStructures #Algorithms #LearningInPublic
