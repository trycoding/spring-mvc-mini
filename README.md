Spring-mvc-mini is a mini project using Spring MVC.

Spring-mvc-mini是一个轻量的项目，基于Spring MVC.

 下面是Spring MVC的Guide页面，这个项目很多是基于它编写的。
 
 http://spring.io/guides


-------------------	
In this project, you can see the code of:

在这个项目里主要实现了以下技术：
* spring-webmvc
* svnkit
* javax.mail
* jasypt
* dom4j
* spring scheduler

To run the application:
如何运行：
-------------------	
From the command line with Maven:

在Windows的CMD：

    $ cd spring-mvc-mini
    $ mvn tomcat7:run [-Dmaven.tomcat.port=<port no.>] (In case 8080 is busy] 

To contribute to this project:

如果你想要学习或贡献和这个项目：

就通过maven把它build成一个Eclipse项目，执行以下命令，打开CMD：

In your preferred IDE such as Eclipse:

    $ cd spring-mvc-mini
    $ mvn eclipse:eclipse

通过Eclipse导入即可。

Import spring-mvc-mini as a Maven Project

通过浏览器打开：http://localhost:8080/spring-mvc-mini

Access the deployed web application at: http://localhost:8080/spring-mvc-mini

Note:
-------------------

 如果你要在Linux环境运行，以下的文件需要修改。

If you want to deploy this project to Linux server, you might need to edit conf files:

    $ spring-oss-mini\src\main\webapp\WEB-INF\spring\appServlet\servlet-context.xml:<context:property-placeholder 
	$ location="file:/opt/web/spring-mvc-mini/resources/application.properties"/>
	$ spring-oss-mini\src\main\resources\logback.xml
	$ spring-oss-mini\resources\application.properties

 最后通过Maven build一个war包部署即可。


