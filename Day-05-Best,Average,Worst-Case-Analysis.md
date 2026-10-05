Day 5 — Best, Average & Worst Case Analysis

📚 What I Learned

Today I learned how to analyze an algorithm based on different possible input situations:

- Best Case — The algorithm performs the minimum amount of work.
- Average Case — The algorithm performs a typical/expected amount of work.
- Worst Case — The algorithm performs the maximum amount of work.

🔎 Example: Linear Search

For a list of "n" elements:

Case| Situation| Time Complexity
Best Case| Target is the first element| O(1)
Average Case| Target is somewhere around the middle| O(n)
Worst Case| Target is the last element or absent| O(n)

Python Example

def linear_search(numbers, target):
    for i in range(len(numbers)):
        if numbers[i] == target:
            return i
    return -1

Example

numbers = [10, 20, 30, 40, 50]
target = 10

The target is found immediately, so this represents the Best Case: O(1).

If the target is near the middle, the algorithm performs approximately "n/2" comparisons, which is still O(n).

If the target is the last element or is not present, the algorithm may examine all "n" elements, giving the Worst Case: O(n).

💡 Key Takeaways

1. Best, average, and worst cases describe different input situations.
2. Best Case represents minimum work.
3. Worst Case represents maximum work.
4. Linear Search has "O(1)" Best Case and "O(n)" Average/Worst Case.
5. Worst-case analysis is important for understanding how an algorithm behaves with difficult inputs.
6. Constants are ignored in Big O, so "O(n/2)" becomes "O(n)".

