# appendix C Configuration properties
# 附录C 配置属性

Although Spring Boot handles a lot of the grunt work when it comes to configuring the components in your application, you may want to fine-tune some of those components. That’s where configuration properties come in handy.  
虽然Spring Boot在应用程序配置组件时处理了很多“粗活”，但你可能还是想对其中某些组件进行微调。这时就该配置属性登场了。

第3章介绍了`@ConfigurationProperties`注解，以及它是如何将配置在代码外部的属性暴露出来的。正如你可以在你创建的组件上使用`@ConfigurationProperties`注解那样，很多Spring Boot自动配置的组件也添加了`@ConfigurationProperties`注解，可以通过Spring Boot支持的各种属性源对其进行配置。
例如，要指定内嵌的Tomcat或Jetty服务器要监听的端口，就可以设置`server.port`属性。这个属性可以设置在application.properties、application.yml、操作系统环境变量，或者是3.2节列出的其他地方里。
本附录列出了Spring Boot组件提供的全部配置属性。请注意，这些属性的是否生效要取决于对应的组件是否被声明为Spring应用程序上下文里的Bean（基本是自动配置的），设置一个不生效组件的属性是没用的。

* `flyway.baseline-description`  
