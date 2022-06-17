[HJ4 字符串分隔](https://www.nowcoder.com/practice/d9162298cb5a437aad722fccccaae8a7)

```java
/*
描述
输入一个字符串，请按长度为8拆分每个输入字符串并进行输出；
长度不是8整数倍的字符串请在后面补数字0，空字符串不处理。

输入描述：
连续输入字符串(每个字符串长度小于等于100)

输出描述：
依次输出所有分割后的长度为8的新字符串

示例1
输入：abc
输出：abc00000
*/

import java.util.*;
public class Main {
    public static void main(String[] args){
        Scanner in = new Scanner(System.in);
        while(in.hasNext()){
            String str = in.nextLine();
            while(str.length() > 8){
                System.out.println(str.substring(0,8));
                str = str.substring(8);
            }
            while(str.length() < 8 && str.length() > 0){
                str += "0";
            }
            System.out.println(str);
        }
    }
}

```

