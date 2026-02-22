# LeetCode Solutions

This repository contains my LeetCode problem solutions written in Python (and later Go).  
The goal is to improve algorithmic thinking and write clean, efficient code.

---

#  Problem: Two Sum

## Problem Summary

Given an integer array `nums` and an integer `target`,  
return the indices of the two numbers such that they add up to `target`.

- Each input has exactly one valid solution.
- The same element cannot be used twice.
- The answer can be returned in any order.

---

## Examples

### Example 1
Input:
nums = [2,7,11,15]  
target = 9  

Output:
[0,1]

Explanation: nums[0] + nums[1] == 9

---

### Example 2
Input:
nums = [3,2,4]  
target = 6  

Output:
[1,2]

---

### Example 3
Input:
nums = [3,3]  
target = 6  

Output:
[0,1]

---

## 📏 Constraints

- 2 ≤ nums.length ≤ 10⁴  
- -10⁹ ≤ nums[i] ≤ 10⁹  
- -10⁹ ≤ target ≤ 10⁹  
- Only one valid answer exists  
