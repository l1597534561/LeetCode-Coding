# **136. Single Number**

### 題目

Given an array of integers, every element appears twice except for one. Find that single one.

### 範例

Your algorithm should have a linear runtime complexity. Could you implement it without using extra memory?

### **解答**

```
public class Solution {
    public int singleNumber(int[] nums) {
        int ans=0;
        for(int k:nums){
            ans=ans^k;
        }
        return ans;
    }
}
```



