[HJ5 进制转换](https://www.nowcoder.com/practice/8f3df50d2b9043208c5eed283d1d4da6)

```java
/*
描述
写出一个程序，接受一个十六进制的数，输出该数值的十进制表示。

数据范围：保证结果在 1≤n≤2^31 − 1 

输入描述：
输入一个十六进制的数值字符串。

输出描述：
输出该数值的十进制字符串。不同组的测试用例用\n隔开。

示例1
输入：0xAA
输出：170
*/

import java.util.*;
public class Main {
    public static void main(String[] args){
        Scanner in = new Scanner(System.in);
        while(in.hasNext()){
            String str = in.nextLine();
            int decimal = Integer.parseInt(str.substring(2,str.length()),16);
            System.out.println(decimal);
        }
    }
}

```

