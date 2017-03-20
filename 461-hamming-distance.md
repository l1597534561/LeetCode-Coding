# **461. Hamming Distance**

### 題目

The Hamming distance between two integers is the number of positions at which the corresponding bits are different.

Given two integers x and y, calculate the Hamming distance.

Note:

0 ≤ x, y &lt; 231.

### 範例

Input: x = 1, y = 4

Output: 2

### 解答

```
public class Solution {
    public int hammingDistance(int x, int y) {
return Integer.bitCount(x ^ y);
      }
}
```



