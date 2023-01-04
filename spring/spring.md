### 1、AnnotationMetadata

```
描述：对类注解信息的提取类
```

![AnnotationMetadata](.\image\AnnotationMetadata.png)



### 2、DeferredImportSelector和ImportSelector

https://blog.csdn.net/boling_cavalry/article/details/82555352

```
作用：实现selectImports方法，可以自定义引入bean
```

```
源码：ConfigurationClassParser的parse(Set<BeanDefinitionHolder> configCandidates)方法
```

```
区别：
a）ImportSelector实例的selectImports方法的执行时机
	在@Configguration注解中的其他逻辑被处理之前，所谓的其他逻辑，包括对@ImportResource、@Bean这些注解的处理（注意，这里只是对@Bean修饰的方法的处理，并不是立即调用@Bean修饰的方法，这个区别很重要！）；

b）DeferredImportSelector实例的selectImports方法的执行时机
	在@Configguration注解中的其他逻辑被处理完毕之后，所谓的其他逻辑，包括对@ImportResource、@Bean这些注解的处理；
```

![ImportSelector](.\image\ImportSelector.png)

![DeferredImportSelector](.\image\DeferredImportSelector.png)

![Configuration](.\image\Configuration.png)



### 3、springboot获取自动配置类

```
主要会去找两个文件：
a）META-INF/spring.factories
b）META-INF/spring/org.springframework.boot.autoconfigure.AutoConfiguration.imports
```

![image-20221119020230893](C:\Users\lenovo\AppData\Roaming\Typora\typora-user-images\image-20221119020230893.png)