# **344. Reverse String**

### 解題

```
public class Solution {
    public String reverseString(String s) {
       StringBuilder bb=new StringBuilder();
        for(int i=s.length();i>0;i--){
            String app=s.substring(i-1,i);
           bb.append(app);
        }   
        return bb.toString();
        
    }
}
```



