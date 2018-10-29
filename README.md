## Welcome to Apache Tomcat!

### Idea中配置tomcat并运行

如果需要idea中运行tomcat程序，需要添加如下配置：
在idea中新建Application，指定启动类为：org.apache.catalina.startup.Bootstrap
启动参数为:-Dcatalina.home="{在本地系统的路径}\tomcat\catalina-home"
1、首先配置pom文件，然后点击导入maven工程，然后点击install即可。
2、启动应用程序，然后再浏览器输入http://localhost:8080/mh/之后，如果可以看到Hello
信息，那么说明tomcat启动成功。（也许你会看到启动报错，那个是正常的，因为webappclassloader
没有加载到webapps下面的事例的class文件，因为下面的文件都是java源文件，所以无法加载）
3、可以把自己项目的class文件放入到webapps，这样是可以访问的。

### 源码解读博客
tomcat源码解读相关的文档将会发布到博客http://47777205.com/ ，感兴趣的可以关注该博客。

### What Is It?

The Apache Tomcat® software is an open source implementation of the Java
Servlet, JavaServer Pages, Java Expression Language and Java WebSocket
technologies. The Java Servlet, JavaServer Pages, Java Expression Language and
Java WebSocket specifications are developed under the
[Java Community Process](http://jcp.org/en/introduction/overview).

The Apache Tomcat software is developed in an open and participatory
environment and released under the
[Apache License version 2](http://www.apache.org/licenses/). The Apache Tomcat
project is intended to be a collaboration of the best-of-breed developers from
around the world. We invite you to participate in this open development
project. To learn more about getting involved,
[click here](http://tomcat.apache.org/getinvolved.html) or keep reading.

Apache Tomcat software powers numerous large-scale, mission-critical web
applications across a diverse range of industries and organizations. Some of
these users and their stories are listed on the
[PoweredBy wiki page](http://wiki.apache.org/tomcat/PoweredBy).

Apache Tomcat, Tomcat, Apache, the Apache feather, and the Apache Tomcat
project logo are trademarks of the Apache Software Foundation.

### The Latest Version

The current latest version in this branch (trunk) can be found on the [Tomcat 9.0](https://tomcat.apache.org/download-90.cgi) page.

### Documentation

The documentation available as of the date of this release is
included in the docs webapp which ships with tomcat. You can access that webapp
by starting tomcat and visiting http://localhost:8080/docs/ in your browser.
The most up-to-date documentation can be found at
http://tomcat.apache.org/tomcat-9.0-doc/.

### Installation

Please see [RUNNING.txt](RUNNING.txt) for more info.

### Licensing

Please see [LICENSE](LICENSE) for more info.

### Support and Mailing List Information

* Free community support is available through the
[tomcat-users](http://tomcat.apache.org/lists.html#tomcat-users) email list and
a dedicated [IRC channel](http://tomcat.apache.org/irc.html) (#tomcat on
Freenode).

* If you want freely available support for running Apache Tomcat, please see the
resources page [here](http://tomcat.apache.org/findhelp.html).

* If you want to be informed about new code releases, bug fixes,
security fixes, general news and information about Apache Tomcat, please
subscribe to the
[tomcat-announce](http://tomcat.apache.org/lists.html#tomcat-announce) email
list.

* If you have a concrete bug report for Apache Tomcat, please see the
instructions for reporting a bug
[here](http://tomcat.apache.org/bugrepo：rt.html).

### Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for more info.
