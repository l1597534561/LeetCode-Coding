# **292. Nim Game**

### 題目

You are playing the following Nim Game with your friend: There is a heap of stones on the table, each time one of you take turns to remove 1 to 3 stones. The one who removes the last stone will be the winner. You will take the first turn to remove the stones.

Both of you are very clever and have optimal strategies for the game. Write a function to determine whether you can win the game given the number of stones in the heap.

For example, if there are 4 stones in the heap, then you will never win the game: no matter 1, 2, or 3 stones you remove, the last stone will always be removed by your friend.

### 想法

NimGame遊戲規則：兩人輪流取石頭，每次要拿一至三個石頭，最後將石頭拿光的人贏得此遊戲。

題目要求玩家1先攻，每位玩家可拿1~3個石頭，玩家1取得最後的石頭獲勝\(True\)，反之則失敗\(False\)，問在幾n個石頭情況下，你會不會贏得遊戲。

### 解答

```
public class Solution {
    public boolean canWinNim(int n) {
        if(n<4){
            return true;
        }else if(n==4){
            return false;
        }else{
            return n%4!=0;
        }
    }
}
```



