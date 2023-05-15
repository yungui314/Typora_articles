- char类型

- - 

```java
public class DataTypeTest01
{
    public static void main(String[] args){
        //定义一个char类型的变量，起名c，同时赋值字符'a'
        char c='a';
        System.out.println(c);
    
    //一个中文字符占2个字节，char类型正好是2个字节
    //所以java中的char类型变量可以存储一个中文字符
    char x='国';
    System.out.println(x);
    }
}
```

- - 转义字符 \

```java
public class DataTypeTest01
{
    public static void main(String[] args){
        //普通的n字符
        char c1='n';
        System.out.println(c1);
        
        char c2='\n';
        System.out.println(c2);
        
        //若想要输出反斜杠字符？
        //反斜杠将后面的单引号字符转义成不具备特殊含义的单引号字符，左边的单引号缺少了结束的单引号字符，编译报错
        /*
        char c3='\';
        System.out.println(c3);
        */
        
        //这样就可以了，第一个\将第二个转义成普通的\
        char c4='\\';
        System.out.println(c4);
        
        //在控制台输出一个单引号？
        char c5='\'';//同上原理
        System.out.println(c5);
        
        //控制台输出半角双引号的"Hello World!"?
        System.out.println("\"Hello World!\"");
        
        char m='中';
        System.out.println(m);
        
        //JDK中自带的native2ascii.exe命令，可以将文字转换成unicode编码
    }
}
```

- - - \n  换行符
    - \t  制表符(tab)
    - \\  普通的\
    - \'  普通的'
    - \"  普通的双引号

  - 转义字符出现在特殊字符前，会将特殊字符转换成普通字符