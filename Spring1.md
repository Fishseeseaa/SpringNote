### Spring IOC
##### 控制反转
##### 管理对象及对象的关系，降低他们的耦合度
##### IOC是其他功能的基础
##### Spring容器是IOC的核心
### Spring AOP
##### 面向切面(方面)编程
##### Filter可以统一处理多个Servlet共同的业务
##### AOP可以统一处理一切对象的共同业务
##### AOP可以降低共同业务和对象之间的耦合度
### Spring MVC
##### 自动实现MVC，给代码分层
##### 进一步降低Servlet与JSP内部的耦合度

### Spring 整合
##### Spring可以管理JDBC，提高开发效率
##### Spring可以整合MyBatis、Hibernate，提高开发效率
##### Spring可以整合Struts2，提高开发效率
##### Spring可以降低这些技术中写信对象的耦合度

## Spring容器
#### 在Spring中，任何的Java类和JavaBean都被当成Bean处理，这些Bean通过容器管理和使用。
#### Spring容器实现了IOC和AOP机制，这些机制可以简化Bean对象创建和Bean对象之间的解耦；
#### Spring容器有BeanFactory和ApplicationContext两种类型

## Bean的命名
#### Bean的名称
在Spring容器中，每个Bean都需要有个名字(即标识符)，改名字可以用<bean>元素的id或name属性指定

#### 的别名
为已定好的Bean，再增加另外一个名字引用，可以使用<alias>指定

    <alias name="fromName" alias="toName"/>
