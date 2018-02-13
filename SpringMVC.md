# SpringMVC
## SpringMVC是什么?
用来简化Web应用开发的mvc框架。
## 五大组件
1.DispatcherServlet(前端控制器)<br/>
2.HandlerMapping<br/>
3.Controller(处理器{业务逻辑，并不是真正的控制层})<br/>
4.ModelAndView<br/>
5.ViewResolver(视图解析器)<br/>
说明：<br/>
step1.前端控制器收到请求之后，依据HandlerMapping的配置，调用响应的Controller来处理。<br/>
step2.Controller(处理器)将处理结果封装成ModelAndView对象，返回给前端控制器。<br/>
注：ModelAndView对象里面通过包含两部分信息（处理结果和视图名，视图名是一个字符串，需要由试图解析器解析成相应的试图对象，比如一个jsp）。<br/>
step3.前端控制器依据视图解析器的解析，调用相应的试图对象(比如事一个jsp)来对处理结果进行展现。<br/>

## 编程步骤
step1.导包(springmvc相关的jar文件).<br/>
step2.添加spring配置文件(比如applicationContext.xml).<br/>
step3.配置前端控制器(web.xml).<br/>
step4.写Controller(处理器).<br/>
step5.写jsp。<br/>
step6.在spring配置文件当中，配置HandlerMapping和ViewResolver。<br/>

## 基于注解SpringMVC应用
step1.导包(springmvc相关的jar文件).<br/>
step2.添加spring配置文件(比如applicationContext.xml).<br/>
step3.配置前端控制器(web.xml).<br/>
