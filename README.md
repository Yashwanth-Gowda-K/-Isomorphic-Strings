# -Isomorphic-Strings


## Problem Description
Given two strings `s` and `t`, determine if they are isomorphic. Two strings are isomorphic if the characters in `s` can be replaced to get `t` with a consistent one-to-one character mapping.

## Solution Approach
This solution uses two hash maps to track character mappings in both directions:
- `s_to_t` maps characters from string `s` to `t`
- `t_to_s` maps characters from string `t` to `s`

The algorithm ensures:
1. No two characters map to the same character (bijection)
2. All character mappings are consistent throughout the strings

## Complexity Analysis
- **Time Complexity**: O(n) - We process each character exactly once
- **Space Complexity**: O(1) - Storage is limited by the fixed character set size

## How to Use
```python
solution = Solution()
print(solution.isIsomorphic("egg", "add"))   # True
print(solution.isIsomorphic("foo", "bar"))   # False
print(solution.isIsomorphic("paper", "title")) # True
