# 13. Roman to Integer

## Problem
Convert a Roman numeral to an integer.

Roman numerals are represented by seven symbols:

| Symbol | Value |
|--------|------|
| I      | 1    |
| V      | 5    |
| X      | 10   |
| L      | 50   |
| C      | 100  |
| D      | 500  |
| M      | 1000 |

Subtraction rules:
- I before V (5) and X (10) → 4, 9  
- X before L (50) and C (100) → 40, 90  
- C before D (500) and M (1000) → 400, 900  

---

## Examples

### Example 1
Input: s = "III"  
Output: 3  
Explanation: III = 3  

### Example 2
Input: s = "LVIII"  
Output: 58  
Explanation: L = 50, V = 5, III = 3  

### Example 3 (Key Case)
Input: s = "MCMXCIV"  
Output: 1994  
Explanation: M(1000) + CM(900) + XC(90) + IV(4)  

---

## Approach
- Use a hashmap (dictionary) to store Roman numeral values
- Traverse the string from left to right
- If the current value is smaller than the next value → subtract
- Otherwise → add to the total

---

## Key Insight
Roman numerals use subtraction when a smaller value appears before a larger one.

---

## Complexity
- Time Complexity: O(n)  
- Space Complexity: O(1)  

---

## Code
```python
class Solution:
    def romanToInt(self, s: str) -> int:
        roman = {
            'I': 1,
            'V': 5,
            'X': 10,
            'L': 50,
            'C': 100,
            'D': 500,
            'M': 1000
        }

        total = 0

        for i in range(len(s)):
            if i + 1 < len(s) and roman[s[i]] < roman[s[i + 1]]:
                total -= roman[s[i]]
            else:
                total += roman[s[i]]
        return total
