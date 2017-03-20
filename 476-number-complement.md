# 476. Number Complement

### 題目

Given a positive integer, output its complement number. The complement strategy is to flip the bits of its binary representation.

### 範例

```
Input: 5
Output: 2
Explanation: The binary representation of 5 is 101 (no leading zero bits), and its complement is 010. So you need to output 2.
```

### 做法

\(非位元做法\)

舉例:

0110 二進位 轉為十進位為6

1001 二進位 轉為十進位為9\(該return的值\)

0110+1001=1111 二進位 轉為十進位為15\(2⁰+2¹+2²+2³\)

15-6=9

在程式碼內

`c+=Math.pow(2,x);`

就是在做2⁰+2¹+2²+2³+....，如果相加結果大於num則會跳離while迴圈

最後將總和減去num為答案。

### 解答

```
public class Solution {
    public int findComplement(int num) {
        int sum=0;
        int x=0;
        while(sum<num){
           sum+=Math.pow(2,x); 
           x++;
        }
        return sum-num;
    }
}
```



$$x = y$$

