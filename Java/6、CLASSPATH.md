- 打开dos窗口，执行java HelloWorld，执行原理？

- - java.exe命令会启动JVM
  - JVM启动之后会启动类加载器ClassLoader
  - ClassLoader会在硬盘上的某个位置搜索HelloWorld.class字节码文件
  - 找到文件则执行
  - 找不到则报错

- 提问：ClassLoader是在哪个位置搜索HelloWorld.class字节码文件的？

- - 默认情况下，ClassLoader从当前路径下加载xxx.class字节码文件

  - 也可以让ClassLoader去某个指定的路径下加载字节码文件，这时需要配置环境变量classpath

  - classpath是给ClassLoader指路的

  - 设置这样的环境变量classpath=D:\……(HelloWorld源文件所在的目录)，此时再打开dos窗口在任意位置，都可以执行:java HelloWorld

  - classpath环境变量没有配置的话，类加载器默认从当前路径下找字节码文件

  - 综上所述，环境变量classpath不再配置，这样类加载器会自动从当前路径下加载class字节码文件。所以，每执行一次.class程序的时候，需要在dos命令窗口中先切换到.class字节码文件所在的路径下，然后运行

  - 当然，classpath也可以这样配置:classpath = **.** 

  - - 路径中".."表示上级目录
    - 路径中"."表示当前目录