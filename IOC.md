## IoC概念
#### IOC全称是Inversion of Control，被译为控制反转；
#### IoC是指程序中对象的获取方式发生反转，由最初的new方式创建，转变为由第三方框架创建、注入(DI)，它降低了对象之间的耦合度。
#### Spring容器是采用DI方式实现了IOC控制，IOC是Spring框架的基础和核心。
## DI
#### DI全称是Dependency Injection，被译为依赖注入;
#### DI的基本原理就是将一起工作具有关系的对象，通过构造方法参数或方法参数传入建立关联，因此容器的工作就是创建bean时注入那些依赖关系。
#### IOC是一种思想，而DI是实现IOC的主要技术途径。
#### DI主要有两种注入方式，即Setter注入和构造器注入。
## Setter注入
#### 通过调用无参构造器或无参static工厂方法实例化bean之后，调用该bean的setter方法，即可实现setter方式的注入。
## 构造器注入
#### 基于构造器的注入是通过调用带参数的构造器来实现的，容器在bean被实例化的时候，根据参数类型执行相应的构造器。
## 自动装配
#### Spring IoC容器可以自动zhaungpei(autowire)相互协作bean之间的关联关系，autowire可以针对单个bean进行设置，autowire的方便指出在于减少xml的注入配置。
#### 在xml配置文件中，可以在<bean/>元素中使用autowire属性指定自动装配规则，一共有五种类型
#### 
