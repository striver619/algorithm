[HJ9 提取不重复的整数](https://www.nowcoder.com/practice/253986e66d114d378ae8de2e6c4577c1)

```java
/*
描述
输入一个 int 型整数，按照从右向左的阅读顺序，返回一个不含重复数字的新的整数。
保证输入的整数最后一位不是 0 。

数据范围： 1 ≤ n ≤ 10^8
  
输入描述：
输入一个int型整数

输出描述：
按照从右向左的阅读顺序，返回一个不含重复数字的新的整数

示例1
输入：9876673
输出：37689

*/

import java.util.*;
public class Main {
    public static void main(String[] args){
        Scanner in = new Scanner(System.in);
        HashSet<Integer> hs = new HashSet<>();
        while(in.hasNext()){
            String str = in.next();
            for(int i=str.length()-1;i>=0;i--){
                Character c = str.charAt(i);
                int n = Integer.parseInt(String.valueOf(c));
                if(hs.add(n)){
                    System.out.print(n);
                }
            }
        }
    }
}


```
