# apache-tomcat-8.5.61-src

下载项目直接到D盘根目录，以下配置直接copy使用

## 入口类
org.apache.catalina.startup.Bootstrap


## VM
-Dcatalina.home=D:/apache-tomcat-8.5.61-src/home

-Dcatalina.base=D:/apache-tomcat-8.5.61-src/home

-Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager

-Djava.util.logging.config.file=D:/apache-tomcat-8.5.61-src/home/conf/logging.properties


## 源码修改
在tomcat的源码ContextConfig.java中的configureStart()函数中手动将JSP解析器初始化： 

context.addServletContainerInitializer(new JasperInitializer(), null); 

 
