![image-20230515134440081](C:\Users\mengxi\AppData\Roaming\Typora\typora-user-images\image-20230515134440081.png)

- Java程序运行包含两个重要的阶段

- - 编译阶段
  - 运行阶段

- 编译阶段

- - 编译阶段主要的任务是检查Java源程序是否符合Java语法，符合则能够生成正常的字节码文件。

  - 字节码文件中不是纯粹的二进制，无法在操作系统中直接执行。

  - 编译阶段的过程：

  - - 在硬盘某个位置新建一个.java扩展名的文件，该文件被称为Java源文件，源文件中编写的是Java源代码/源程序。

    - 需要使用JDK中自带的javac.exe命令进行Java程序的编译。

    - - javac怎么用？

      - - 在dos命令窗口使用。
        - 使用规则：javac java源文件的路径

      - javac是一个java编译器工具/命令。

    - 一个java源文件可以编译生成多个.class文件。

    - 字节码文件/class文件是最终要执行的文件，所以说class文件生成之后，java源文件删除并不会影响java程序的执行。

    - 编译结束可以将class文件拷贝到其他操作系统当中。(跨平台)

- 运行阶段【跨平台】

- - JDK还自带一个工具/命令，叫java.exe。java.exe主要负责运行阶段。

  - java.exe怎么用？

  - - 在dos窗口使用。
    - 使用方法：java 类名。注意不是路径。

  - 运行阶段过程：

  - - 打开dos命令窗口。
    - 输入：java A。
    - java.exe会启动JVM，JVM会启动类加载器ClassLoader。
    - ClassLoader会去硬盘上搜索A.class文件，找到后将该字节码文件装载到JVM当中。
    - JVM将A.class字节码文件解释成二进制1010100101这样的数据。
    - 然后操作系统执行二进制和底层硬件平台进行交互。