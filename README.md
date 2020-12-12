# apache-tomcat-8.5.61-src

org.apache.catalina.startup.Bootstrap



-Dcatalina.home=D:/apache-tomcat-8.5.61-src/home

-Dcatalina.base=D:/apache-tomcat-8.5.61-src/home

-Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager

-Djava.util.logging.config.file=D:/apache-tomcat-8.5.61-src/home/conf/logging.properties



在tomcat的源码ContextConfig.java

中的configureStart()函数中手动将JSP解析器初始化： 

context.addServletContainerInitializer(new JasperInitializer(), null); 

 