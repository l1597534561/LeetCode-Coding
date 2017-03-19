# **461. Hamming Distance**

### 解答

```
public class Solution {
    public int hammingDistance(int x, int y) {
return Integer.bitCount(x ^ y);
      }
}
```



