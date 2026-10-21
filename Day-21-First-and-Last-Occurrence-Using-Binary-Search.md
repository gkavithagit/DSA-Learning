Day 21: First and Last Occurrence Using Binary Search

📌 Today's Topic

Finding the first and last occurrences of a target element in a sorted array using Binary Search.

🎯 Learning Objectives

- Understand how to find the first occurrence of an element.
- Understand how to find the last occurrence of an element.
- Apply binary search to solve array problems efficiently.
- Understand time and space complexity.

🧠 Concept Explanation

Binary Search is an efficient searching algorithm that works on sorted arrays by repeatedly dividing the search space into two halves.

When duplicate elements exist, normal binary search may find any occurrence of the target. To find the first or last occurrence, we modify the algorithm.

1. First Occurrence

When the target is found:

- Store its index as the current answer.
- Continue searching in the left half.
- Update the answer if an earlier occurrence is found.

2. Last Occurrence

When the target is found:

- Store its index as the current answer.
- Continue searching in the right half.
- Update the answer if a later occurrence is found.

If the target does not exist, the functions return "-1".

💻 Python Implementation

def find_first(arr, target):
    left, right = 0, len(arr) - 1
    answer = -1

    while left <= right:
        mid = (left + right) // 2

        if arr[mid] == target:
            answer = mid
            right = mid - 1
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1

    return answer


def find_last(arr, target):
    left, right = 0, len(arr) - 1
    answer = -1

    while left <= right:
        mid = (left + right) // 2

        if arr[mid] == target:
            answer = mid
            left = mid + 1
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1

    return answer


arr = [1, 2, 2, 2, 3, 4, 5]
target = 2

print("First occurrence:", find_first(arr, target))
print("Last occurrence:", find_last(arr, target))

📤 Output

First occurrence: 1
Last occurrence: 3

⏱️ Time and Space Complexity

Operation| Complexity
First occurrence| O(log n)
Last occurrence| O(log n)
Auxiliary space| O(1)

Time Complexity: O(log n), because the search space is approximately halved in each iteration.

Space Complexity: O(1), because the iterative algorithms use only a constant amount of additional memory.

💡 Key Takeaways

- Binary Search requires a sorted array.
- Finding the first occurrence requires continuing the search to the left.
- Finding the last occurrence requires continuing the search to the right.
- Saving the answer before continuing is essential.
- Returning "-1" indicates that the target was not found.

✅ Day 21 Progress

- Studied first and last occurrence using Binary Search.
- Practised Python implementation.
- Reviewed time and space complexity.
- Completed the concept quiz with a score of 5/5.

🚀 Next Goal

Continue practising DSA problems to improve logical thinking, coding skills, and placement interview preparation.
