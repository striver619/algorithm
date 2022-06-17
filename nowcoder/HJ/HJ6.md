[HJ6 质数因子](https://www.nowcoder.com/practice/196534628ca6490ebce2e336b47b3607)

```java
/*
描述

功能:输入一个正整数，按照从小到大的顺序输出它的所有质因子（重复的也要列举）（如180的质因子为2 2 3 3 5 ）


数据范围： 1 ≤ n ≤ 2 * 10^{9} + 14 

输入描述：
输入一个整数

输出描述：
按照从小到大的顺序输出它的所有质数的因子，以空格隔开。

示例1
输入：180
输出：2 2 3 3 5
*/

import java.util.*;
public class Main {
    public static void main(String[] args){
        Scanner in = new Scanner(System.in);
        while(in.hasNext()){
            int num = in.nextInt();
            int x = 2;
            while(num != 1){
                if(num % x == 0){
                    System.out.print(x + " ");
                    num /= x;
                }else{
                    if(x > num/x){
                        x = num;
                    }else{
                        x++;
                    }
                }
            }
        }
    }
}
```

