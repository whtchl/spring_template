# spring_template

1. 这套代码中可以借鉴如何使用JunitTest



2. Bean的注入： 
构造 注入

 
设值注入
 
3. Bean的作用域


4. Bean的两种初始化方式


5. bean的销毁两种方式

6.配置全局的默认初始化和销毁方法


7.初始化销毁的顺序
InitializingBean,DisposableBean的 afterPropertiesSet ，destroy方法优先于
 <bean id="beanLifeCycle" class="com.imooc.lifecycle.BeanLifeCycle"  init-method="start" destroy-method="stop"></bean>  中的start 和stop。
 
 下面的全局默认初始化和销毁方法当有上面的两种中的其中一种方法时，全局的方法不再执行。
 <beans xmlns="http://www.springframework.org/schema/beans"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://www.springframework.org/schema/beans
        http://www.springframework.org/schema/beans/spring-beans.xsd" 
  default-init-method="defautInit" default-destroy-method="defaultDestroy" >
 
 
