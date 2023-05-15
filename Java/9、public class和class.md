- public class和class区别？

- - 一个java源文件可以定义多个class

  - 一个java源文件中public的class不是必须的

  - 一个class会对应生成一个xxx.class字节码文件

  - **一个java源文件当中定义公开的类的话，public的class只能有一个，并且该类名必须与java名称一致**

  - 每一个class当中都可以编写main方法，都可以设定程序的入口，想执行B.class中的main方法：

  - - java B

  - 注意：当在命令窗口中执行java Hello，那么要求Hello.class必须有主方法。没有主方法会出现运行阶段的错误

  - - 错误提示：错误: 在类 B 中找不到 main 方法, 请将 main 方法定义为:

​				     public static void main(String[] args)

​					 否则 JavaFX 应用程序类必须扩展javafx.application.Application