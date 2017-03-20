# 231. Power of Two

### 題目

Given an integer, write a function to determine if it is a power of two.

### 範例

input:4

output:true

### 作法

### 解答

```
public class Solution {
    public boolean isPowerOfTwo(int n) {
        boolean isV=false;
        while(n>0){
            if(n%2==0){
                n=n/2;
                if(n==1){
                    isV=true;
                }
            }else if(n==1){
                isV=true;
                break;
            }else{
                break;
            }
        }
        return isV;
    }
}
```



