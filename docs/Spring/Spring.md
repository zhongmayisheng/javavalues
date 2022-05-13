# Spring面试题


~~[说明：提供正版免费激活下载，以及激活工具和教程，点击获取](http://www.idejihuo.com)~~

[![img](https://gitee.com/itmatu/zhongmayisheng/raw/master/video/img/Release_Preview_image_1280x600_IntelliJIDEA-2x.jpg)](http://www.idejihuo.com)


- [Spring面试题](#spring面试题)
  - [目录](#目录)
    - [1、不同版本的 Spring Framework 有哪些主要功能？](#1不同版本的-spring-framework-有哪些主要功能)
    - [2、什么是 Spring Framework？](#2什么是-spring-framework)
    - [3、列举 Spring Framework 的优点。](#3列举-spring-framework-的优点)
    - [4、Spring Framework 有哪些不同的功能？](#4spring-framework-有哪些不同的功能)
    - [5、Spring Framework 中有多少个模块，它们分别是什么？](#5spring-framework-中有多少个模块它们分别是什么)
    - [6、什么是 Spring 配置文件？](#6什么是-spring-配置文件)
    - [7、Spring 应用程序有哪些不同组件？](#7spring-应用程序有哪些不同组件)
    - [8、使用 Spring 有哪些方式？](#8使用-spring-有哪些方式)
    - [9、什么是 Spring IOC 容器？](#9什么是-spring-ioc-容器)
    - [10、什么是依赖注入？](#10什么是依赖注入)
    - [11、可以通过多少种方式完成依赖注入？](#11可以通过多少种方式完成依赖注入)
    - [12、区分构造函数注入和 setter 注入](#12区分构造函数注入和-setter-注入)
    - [13、spring 中有多少种 IOC 容器？](#13spring-中有多少种-ioc-容器)
    - [14、区分 BeanFactory 和 ApplicationContext。](#14区分-beanfactory-和-applicationcontext)
    - [15、列举 IoC 的一些好处。](#15列举-ioc-的一些好处)
    - [16、Spring IoC 的实现机制。](#16spring-ioc-的实现机制)
    - [17、什么是 spring bean？](#17什么是-spring-bean)
    - [18、spring 提供了哪些配置方式？](#18spring-提供了哪些配置方式)
    - [19、spring 支持集中 bean scope？](#19spring-支持集中-bean-scope)
    - [20、spring bean 容器的生命周期是什么样的？](#20spring-bean-容器的生命周期是什么样的)
    - [21、什么是 spring 的内部 bean？](#21什么是-spring-的内部-bean)
    - [22、什么是 spring 装配](#22什么是-spring-装配)
    - [23、自动装配有哪些方式？](#23自动装配有哪些方式)
    - [24、自动装配有什么局限？](#24自动装配有什么局限)
    - [25、什么是基于注解的容器配置](#25什么是基于注解的容器配置)
    - [26、如何在 spring 中启动注解装配？](#26如何在-spring-中启动注解装配)
    - [27、@Component, @Controller, @Repository](#27component-controller-repository)
    - [28、@Required 注解有什么用？](#28required-注解有什么用)
    - [29、@Autowired 注解有什么用？](#29autowired-注解有什么用)
    - [30、@Qualiﬁer 注解有什么用？](#30qualiﬁer-注解有什么用)
    - [31、@RequestMapping 注解有什么用？](#31requestmapping-注解有什么用)
    - [32、spring DAO 有什么用？](#32spring-dao-有什么用)
    - [更多...](#更多)


---

##  目录

### 1、不同版本的 Spring Framework 有哪些主要功能？

|Version	|Feature|
|---|---|
|Spring 2.5|	发布于 2007 年。这是第一个支持注解的版本。
|Spring 3.0|	发布于 2009 年。它完全利用了 Java5 中的改进，并为 JEE6 提供了支 持
|Spring 4.0|	发布于 2013 年。这是第一个完全支持 JAVA8 的版本。
|Spring 5.0|	Spring Framework 5.0的最大特点之一是响应式编程（Reactive Programming）。 响应式编程核心功能和对响应式endpoints的支持可通过Spring Framework 5.0中获得。


### 2、什么是 Spring Framework？
Spring 是一个开源应用框架，旨在降低应用程序开发的复杂度。它是轻量级、松散耦合的。它具有分层体系结构，允许用户选择组件，同时还为 J2EE 应用程序开发提供了一个有凝聚力的框架。它可以集成其他框架，如 Structs、Hibernate、EJB 等，所以又称为框架的框架。


### 3、列举 Spring Framework 的优点。
由于 Spring Frameworks 的分层架构，用户可以自由选择自己需要的组件。Spring Framework 支持 POJO(Plain Old Java Object) 编程， 从而具备持续集成和可测试性。由于依赖注入和控制反转，JDBC 得以简化。它是开源免费的。


### 4、Spring Framework 有哪些不同的功能？

- 轻量级 - Spring 在代码量和透明度方面都很轻便。
- IOC - 控制反转 
- AOP - 面向切面编程可以将应用业务逻辑和系统服务分离，以实现高内聚。
- 容器 - Spring 负责创建和管理对象（Bean）的生命周期和配置。
- MVC - 对 web 应用提供了高度可配置性，其他框架的集成也十分方便。
- 事务管理 - 提供了用于事务管理的通用抽象层。Spring 的事务支持也可用于容器较少的环境。
- JDBC 异常 - Spring的 JDBC 抽象层提供了一个异常层次结构，简化了错误处理策略。


### 5、Spring Framework 中有多少个模块，它们分别是什么？

[![img](../img/图片43.png)](http://www.idejihuo.com)

- **Spring 核心容器 – 该层基本上是 Spring Framework 的核心。它包含以下模块：**

1) Spring Core
2) Spring Bean
3) SpEL (Spring Expression Language)
4) Spring Context

- **数据访问/集成 – 该层提供与数据库交互的支持。它包含以下模块：**

1) JDBC ( Java DataBase Connectivity)
2) ORM (Object Relational Mapping)
3) OXM (Object XML Mappers)
4) JMS ( Java Messaging Service)
5) Transaction

- **Web – 该层提供了创建 Web 应用程序的支持。它包含以下模块：**

1) Web
2) Web – Servlet 
3) Web – Socket 
4) Web – Portlet

- **AOP**

该层支持面向切面编程

- **nstrumentation**

该层为类检测和类加载器实现提供支持。

- **Test**

该层为使用 JUnit 和 TestNG 进行测试提供支持。

- **几个杂项模块:**

Messaging – 该模块为 STOMP 提供支持。它还支持注解编程模型，该模型用于从 WebSocket 客户端路由和处理 STOMP 消息。

Aspects –该模块为与 AspectJ 的集成提供支持。

### 6、什么是 Spring 配置文件？
Spring 配置文件是 XML 文件。该文件主要包含类信息。它描述了这些类是如何配置以及相互引入的。但是，XML 配置文件冗长且更加干净。如果没有正确规划和编写，那么在大项目中管理变得非常困难

### 7、Spring 应用程序有哪些不同组件？

Spring 应用一般有以下组件：

1) 接口 - 定义功能。
2) Bean 类 - 它包含属性，setter 和 getter 方法，函数等。
3) Spring 面向切面编程（AOP） - 提供面向切面编程的功能。
4) Bean 配置文件 - 包含类的信息以及如何配置它们。
5) 用户程序 - 它使用接口。


### 8、使用 Spring 有哪些方式？
使用 Spring 有以下方式：
1) 作为一个成熟的 Spring Web 应用程序。

作为第三方 Web 框架，使用 Spring Frameworks 中间层。

1) 用于远程使用。
2) 作为企业级 Java Bean，它可以包装现有的 POJO（Plain Old Java Objects）。


### 9、什么是 Spring IOC 容器？
Spring 框架的核心是 Spring 容器。容器创建对象，将它们装配在一起，配置它们并管理它们的完整生命周期。Spring 容器使用依赖注入来管理组成应用程序的组件。容器通过读取提供的配置元数据来接收对象进行实例化，配置和组装的指令。该元数据可以通过 XML，Java 注解或 Java 代码提供。


### 10、什么是依赖注入？
在依赖注入中，您不必创建对象，但必须描述如何创建它们。您不是直接在代码中将组件和服务连接在一起，而是描述配置文件中哪些组件需要哪些服务。由 IoC容器将它们装配在一起。


### 11、可以通过多少种方式完成依赖注入？

通常，依赖注入可以通过三种方式完成，即：

1) 构造函数注入
2) etter 注入
3) 接口注入

在 Spring Framework 中，仅使用构造函数和 setter 注入。


### 12、区分构造函数注入和 setter 注入

|构造函数注入|	setter 注入
|---|---|
|没有部分注入|	有部分注入
|不会覆盖 setter 属性| 	会覆盖 setter 属性
|任意修改都会创建一个新实例|	任意修改不会创建一个新实例
|适用于设置很多属性| 适用于设置少量属性


### 13、spring 中有多少种 IOC 容器？
- BeanFactory - BeanFactory 就像一个包含 bean 集合的工厂类。它会在客户端要求时实例化 bean。
- ApplicationContext - ApplicationContext 接口扩展了 BeanFactory 接口。它在 BeanFactory 基础上提供了一些额外的功能。


### 14、区分 BeanFactory 和 ApplicationContext。

|BeanFactory|	ApplicationContext|
|---|---|
|它使用懒加载|	它使用即时加载|
|它使用语法显式提供资源对象|	它自己创建和管理资源对象|
|不支持国际化|	支持国际化|
|不支持基于依赖的注解|	支持基于依赖的注解|


### 15、列举 IoC 的一些好处。

IoC 的一些好处是：
- 它将最小化应用程序中的代码量。
- 它将使您的应用程序易于测试，因为它不需要单元测试用例中的任何单例或 JNDI 查找机制。
- 它以最小的影响和最少的侵入机制促进松耦合。
- 它支持即时的实例化和延迟加载服务。


### 16、Spring IoC 的实现机制。

Spring 中的 IoC 的实现原理就是工厂模式加反射机制。实例:
```
interface Fruit {
public abstract void eat();
}

class Apple implements Fruit { public void eat(){ System.out.println("Apple");
}
}

class Orange implements Fruit { public void eat(){ System.out.println("Orange");
}
}

class Factory {
public static Fruit getInstance(String ClassName) { Fruit f=null;
try {
f=(Fruit)Class.forName(ClassName).newInstance();
} catch (Exception e) { e.printStackTrace();
}
return f;
}
}
class Client {
public static void main(String[] a) {
Fruit f=Factory.getInstance("io.github.dunwu.spring.Apple"); if(f!=null){
f.eat();
}
```

### 17、什么是 spring bean？
- 它们是构成用户应用程序主干的对象。
- Bean 由 Spring IoC 容器管理。
- 它们由 Spring IoC 容器实例化，配置，装配和管理。
- Bean 是基于用户提供给容器的配置元数据创建。


### 18、spring 提供了哪些配置方式？

**基于 xml 配置**

bean 所需的依赖项和服务在 XML 格式的配置文件中指定。这些配置文件通常包含许多 bean 定义和特定于应用程序的配置选项。它们通常以 bean 标签开头。例如：
```
<bean id="studentbean" class="org.edureka.firstSpring.StudentBean">
<property name="name" value="Edureka"></property>
</bean>
```
**基于注解配置**

您可以通过在相关的类，方法或字段声明上使用注解，将 bean 配置为组件类本身，而不是使用 XML 来描述 bean 装配。默认情况下，Spring 容器中未打开注解装配。因此，您需要在使用它之前在 Spring 配置文件中启用它。例如：

**基于 Java API 配置**

Spring 的 Java 配置是通过使用 @Bean 和 @Conﬁguration 来实现。

1) @Bean 注解扮演与 元素相同的角色。
2)  @Conﬁguration 类允许通过简单地调用同一个类中的其他 @Bean 方法来定义 bean 间依赖关系。

例如：
```
@Configuration
public class StudentConfig { @Bean
public StudentBean myStudent() { return new StudentBean();
}
}
```

### 19、spring 支持集中 bean scope？

Spring bean 支持 5 种 scope：

- Singleton - 每个 Spring IoC 容器仅有一个单实例。
- Prototype - 每次请求都会产生一个新的实例。
- Request - 每一次 HTTP 请求都会产生一个新的实例，并且该 bean 仅在当前 HTTP 请求内有效。
- Session - 每一次 HTTP 请求都会产生一个新的 bean，同时该 bean 仅在当前HTTP session 内有效。
- Global-session - 类似于标准的 HTTP Session 作用域，不过它仅仅在基于portlet 的 web 应用中才有意义
- Portlet 规范定义了全局 Session 的概念，
它被所有构成某个 portlet web 应用的各种不同的 portlet 所共享。在 globalsession 作用域中定义的 bean 被限定于全局 portlet Session
的生命周期范围内。如果你在 web 中使用 global session 作用域来标识 bean，那么 web会自动当成 session 类型来使用。

仅当用户使用支持 Web 的 ApplicationContext 时，最后三个才可用。


### 20、spring bean 容器的生命周期是什么样的？

spring bean 容器的生命周期流程如下：

1) Spring 容器根据配置中的 bean 定义中实例化 bean。
2) Spring 使用依赖注入填充所有属性，如 bean 中所定义的配置。
3) 如果 bean 实现 BeanNameAware 接口，则工厂通过传递 bean 的 ID 来调用setBeanName()。
4) 如果 bean 实现 BeanFactoryAware 接口，工厂通过传递自身的实例来调用 setBeanFactory()。
5) 如果存在与 bean 关联的任何 BeanPostProcessors，则调用 ```preProcessBeforeInitialization()``` 方法。
6) 如果为 bean 指定了 init 方法（ 的 init-method 属性），那么将调用它。
7) 最后，如果存在与 bean 关联的任何 ```BeanPostProcessors```，则将调用 ```postProcessAfterInitialization()``` 方法。
8) 如果 bean 实现DisposableBean 接口，当 spring 容器关闭时，会调用 destory()。
9) 如果为bean 指定了 destroy 方法（ 的 destroy-method 属性），那么将调用它。


### 21、什么是 spring 的内部 bean？
只有将 bean 用作另一个 bean 的属性时，才能将 bean 声明为内部 bean。为了定义 bean，Spring 的基于 XML 的配置元数据在 或 中提供了 元素的使用。内部 bean 总是匿名的，它们总是作为原型。

例如，假设我们有一个 Student 类，其中引用了 Person 类。这里我们将只创建一个 Person 类实例并在 Student 中使用它。

**Student.java**

```
public class Student { private Person person;
//Setters and Getters
}
public class Person { private String name; private String address;
//Setters and Getters
```


**bean.xml**

```
<bean id=“StudentBean" class="com.edureka.Student">
<property name="person">
<!--This is inner bean -->
<bean class="com.edureka.Person">
<property name="name" value=“Scott"></property>
<property name="address" value= “Bangalore"></property>
</bean>
</property>
</bean>
```


### 22、什么是 spring 装配
当 bean 在 Spring 容器中组合在一起时，它被称为装配或 bean 装配。Spring容器需要知道需要什么 bean 以及容器应该如何使用依赖注入来将 bean 绑定在一起，同时装配 bean。


### 23、自动装配有哪些方式？
Spring 容器能够自动装配 bean。也就是说，可以通过检查 BeanFactory 的内容让 Spring 自动解析 bean 的协作者。

**自动装配的不同模式：**

- no - 这是默认设置，表示没有自动装配。应使用显式 bean 引用进行装配。
- byName - 它根据 bean 的名称注入对象依赖项。它匹配并装配其属性与 XML文件中由相同名称定义的 bean。
- byType - 它根据类型注入对象依赖项。如果属性的类型与 XML 文件中的一个 bean 名称匹配，则匹配并装配属性
- 构造函数 - 它通过调用类的构造函数来注入依赖项。它有大量的参数。
- autodetect - 首先容器尝试通过构造函数使用 autowire 装配，如果不能，则尝试通过 byType 自动装配


### 24、自动装配有什么局限？

**覆盖的可能性**

- 您始终可以使用 和 设置指定依赖项，这将覆盖自动装配。基本元数据类型 
- 简单属性（如原数据类型，字符串和类）无法自动装配。令人困惑的性质 
- 总是喜欢使用明确的装配，因为自动装配不太精确。


### 25、什么是基于注解的容器配置
不使用 XML 来描述 bean 装配，开发人员通过在相关的类，方法或字段声明上使用注解将配置移动到组件类本身。它可以作为 XML 设置的替代方案。

例如：Spring 的 Java 配置是通过使用 @Bean 和 @Conﬁguration 来实现。 @Bean 注解扮演与 元素相同的角色。@Conﬁguration 类允许通过简单地调用同一个类中的其他 @Bean 方法来定义 bean 间依赖关系。

例如
```
@Configuration
public class StudentConfig { @Bean
public StudentBean myStudent() { return new StudentBean();
}
}
```

### 26、如何在 spring 中启动注解装配？
默认情况下，Spring 容器中未打开注解装配。因此，要使用基于注解装配，我们必须通过配置 ```<context：annotation-conﬁg/>``` 元素在
Spring 配置文件中启用它。


### 27、@Component, @Controller, @Repository

- **@Service 有何区别？**

- **@Component**：这将 java 类标记为 bean。它是任何 Spring 管理组件的通用构造型。spring 的组件扫描机制现在可以将其拾取并将其拉入应用程序环境中。
- **@Controller**：这将一个类标记为 Spring Web MVC 控制器。标有它的Bean 会自动导入到 IoC 容器中。
- **@Service**：此注解是组件注解的特化。它不会对 @Component 注解提供任何其他行为。您可以在服务层类中使用@Service 而不是 @Component，因为它以更好的方式指定了意图。
- **@Repository**：这个注解是具有类似用途和功能的 @Component 注解的特化。它为 DAO 提供了额外的好处。它将 DAO 导入 IoC 容器， 并使未经检查的异常有资格转换为 Spring DataAccessException。


### 28、@Required 注解有什么用？
@Required 应用于 bean 属性 setter 方法。此注解仅指示必须在配置时使用bean 定义中的显式属性值或使用自动装配填充受影响的 bean 属性。如果尚未填充受影响的 bean 属性，则容器将抛出 ```eanInitializationException```。

示例：
```
public class Employee { private String name; @Required
public void setName(String name){ this.name=name;
}
public string getName(){ return name;
}
}
```


### 29、@Autowired 注解有什么用？
@Autowired 可以更准确地控制应该在何处以及如何进行自动装配。此注解用于在 setter 方法，构造函数，具有任意名称或多个参数的属性或方法上自动装配bean。默认情况下，它是类型驱动的注入。
```
public class Employee { private String name; @Autowired
public void setName(String name) { this.name=name;
}
public string getName(){ return name;
}
}
```


### 30、@Qualiﬁer 注解有什么用？
当您创建多个相同类型的 bean 并希望仅使用属性装配其中一个 bean 时，您可以使用@Qualiﬁer 注解和 @Autowired 通过指定应该装配哪个确切的 bean 来消除歧义。
例如，这里我们分别有两个类，Employee 和 EmpAccount。在 EmpAccount中，使用@Qualiﬁer 指定了必须装配 id 为 emp1 的 bean。

**EmpAccount.java**

```
public class Employee { private String name; @Autowired
public void setName(String name) { this.name=name;
}
public string getName() { return name;
}
}
```

**Employee.java**

```
public class EmpAccount { private Employee emp; @Autowired @Qualifier(emp1)
public void showName() {
System.out.println(“Employee name : ”+emp.getName);
}
}
```


### 31、@RequestMapping 注解有什么用？
@RequestMapping 注解用于将特定 HTTP 请求方法映射到将处理相应请求的控制器中的特定类/方法。此注释可应用于两个级别：
- 类级别：映射请求的 URL 
- 方法级别：映射 URL 以及 HTTP 请求方法


### 32、spring DAO 有什么用？
Spring DAO 使得 JDBC，Hibernate 或 JDO 这样的数据访问技术更容易以一种统一的方式工作。这使得用户容易在持久性技术之间切换。它还允许您在编写代码时，无需考虑捕获每种技术不同的异常。

[![img](../img/图片44.png)](http://www.idejihuo.com)

### 更多...