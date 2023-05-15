- 保证已经安装文本编辑器

- 已经安装了JDK

- JRE：java runtime environment，即java语言运行环境。JVM包含于JRE。

- JDK目录介绍：

- - JDK/bin：该目录下存放了很多命令，如javac、java

- 编写HelloWorld源程序

  

  ```java
  public class HelloWorld {     
  	public static void main(String[] args) {
      	System.out.println("Hello World!");    
      	} 
  }
  ```

- 将HelloWorld.java源程序通过javac工具进行编译：

- - 首先要解决：javac是否可用

  - 打开dos命令窗口，直接输入javac回车，出现   'javac' 不是内部或外部命令，也不是可运行的程序或批处理文件。

  - 出现以上问题是因为：windows操作系统无法找到javac命令文件

  - 如何解决以上问题？

  - - windows如何搜索硬盘上某个命令的呢？

    - - 首先会从当前目录下搜索
      - 如果当前目录搜索不到的话，会从环境变量path指定的路径中搜索某个命令
      - 如果都搜索不到，则报错

  - 配置环境变量path

  - - 注意：path环境变量和Java没有关系。path环境变量是专门给windows操作系统指路的
    - javac若想随意使用，需要将javac所在的文件目录配置到系统环境变量path中

  - javac怎么用？

  - - javac java源文件路径
    - 注意：绝对路径和相对路径都可以

- 运行java程序

- - 需要使用java.exe命令

  - 首先测试java是否可用

  - 使用方法：java 类名

  - - 硬盘上有HelloWorld.class，那么类名就是:  HelloWorld
    - 一定要注意：java后面跟的是类名，不是文件路径

  - 首先需要将dos窗口目录切换到helloworld.class文件所在目录，然后运行