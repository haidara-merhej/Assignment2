# Reverse String

## Problem Link
[Reverse String - LeetCode](https://leetcode.com/problems/reverse-string/)

## Solution

```csharp
public class Solution {
    public void ReverseString(char[] s) {
        int left = 0;
        int right = s.Length - 1;

        while(left < right)
        {
            char temp = s[left];
            s[left] = s[right];
            s[right] = temp;

            left++;
            right--;
        }
    }
}
```

## Approach
I used the Two Pointers technique.
One pointer starts at the beginning of the array, and the other starts at the end.
I swap the characters at both pointers, then move the first pointer forward
and the second pointer backward until they meet.

# Complexity
- **Time complexity:** O(n)
- **Space complexity:** O(1)

## LeetCode Profile

[Visit my leetcode profile](https://leetcode.com/u/Haidara_Merhej/)



