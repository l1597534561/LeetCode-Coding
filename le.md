# **412. Fizz Buzz**

### 題目

Write a program that outputs the string representation of numbers from 1 to n.

But for multiples of three it should output “Fizz” instead of the number and for the multiples of five output “Buzz”. For numbers which are multiples of both three and five output “FizzBuzz”.

### 範例

如果n=15，則會回傳\["1", "2", "Fizz", "4", "Buzz", "Fizz", "7", "8", "Fizz", "Buzz", "11", "Fizz", "13", "14", "FizzBuzz"\]

### 做法

n在3的倍數時會回傳"Fizz"，在5的倍數回傳"Buzz"，如果同時為3和5的倍數時回傳"FizzBuzz"，所以首先判斷是否為3or5的倍數後，再分別判斷3與5的倍數且個別加進list內。

### **解答**

```
public class Solution {
    public List<String> fizzBuzz(int n) {
        int i=1;
        List<String> list=new ArrayList<String>();
        while(i<=n){
        if(i%3==0&&i%5==0){
            list.add("FizzBuzz");
        }else if(i%3==0){
            list.add("Fizz");
        }else if(i%5==0){
            list.add("Buzz");
        }else{
            list.add(Integer.toString(i));
        }
        i++;
        }
        return list;
    }
}
```



