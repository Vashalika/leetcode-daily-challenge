# LeetCode Daily Challenge 🚀

Welcome to my LeetCode Daily Challenge repository!

I am starting my coding journey by solving one
LeetCode problem every day. My goal is to improve
my problem-solving skills and learn Data Structures
and Algorithms (DSA).

## 🎯 Goals

- Solve one problem every day.
- Start with Easy problems.
- Gradually practice Medium and Hard problems.
- Understand the logic behind every solution.
- Track my daily progress on GitHub.

## 📅 Daily Progress

| Day | Date | Problem | Difficulty | Status |
|---|---|---|---|---|
| Day 1 | 2026-10-17 | Two Sum | Easy | Completed |
| Day 2 | TBD | TBD | TBD | Pending |
| Day 3 | TBD | TBD | TBD | Pending |

## 🟢 Day 1: Two Sum

- **LeetCode Number:** 1
- **Difficulty:** Easy
- **Topic:** Array, Hash Table
- **Language:** Python
- **Problem Link:** [Two Sum](https://leetcode.com/problems/two-sum/description/)
- **Solution File:** [two_sum.py](Easy/two_sum.py)

### Problem Description

Given an array of integers and a target value,
find the indices of two numbers whose sum equals
the target.

You cannot use the same element twice.

### Example

Input:
```text
nums = [2, 7, 11, 15]
target = 9
```

Output:
```text
[0, 1]
```

Explanation:

nums[0] + nums[1] = 2 + 7 = 9

Therefore, the answer is [0, 1].

### Approach

1. Create an empty dictionary.
2. Visit each number in the array.
3. Calculate the required number:
   complement = target - current number.
4. Check whether the complement exists in the dictionary.
5. If it exists, return both indices.
6. Otherwise, store the current number and its index.

### Python Solution

```python
class Solution:
    def twoSum(self, nums, target):
        seen = {}

        for i, num in enumerate(nums):
            complement = target - num

            if complement in seen:
                return [seen[complement], i]

            seen[num] = i
```

### Complexity Analysis

- Time Complexity: O(n)
- Space Complexity: O(n)

Here, n is the number of elements in the array.

### What I Learned

- How to use arrays and dictionaries.
- How to find two numbers using a target sum.
- How to return array indices.
- How a hash table can improve efficiency.

## 📈 My Progress

- Total Problems Solved: 1
- Easy: 1
- Medium: 0
- Hard: 0

## 🌱 My Commitment

I will keep updating this repository as I solve
more LeetCode problems every day.

One problem a day, one step closer to my goals! 💻
