https://blog.csdn.net/ShuSheng0007/article/details/107066856

## 1、MethodHandle含义

```
Lookup
	MethodHandle 的创建工厂，通过它可以创建MethodHandle，值得注意的是检查工作是在创建时处理的，而不是在调用时处理。

MethodType
	顾名思义，就是代表方法的签名。一个方法的返回值类型是什么，有几个参数，每个参数的类型什么？

MethodHandle
	方法句柄，通过它我们就可以动态访问类型信息了。

	众所周知，Java从最初发布时就支持反射，通过反射可以在运行时获取类型信息，但其有个缺点就是执行速度较慢。于是从Java 7开始提供了另一套API MethodHandle 。其与反射的作用类似，可以在运行时访问类型信息，但是据说其执行效率比反射更高，也被称为Java的 现代化反射。
```



## 2、MethodHandle作用

- [访问构造函数](https://blog.csdn.net/ShuSheng0007/article/details/107066856#_144)
- [访问非private实例方法](https://blog.csdn.net/ShuSheng0007/article/details/107066856#private_156)
- [访问private实例方法](https://blog.csdn.net/ShuSheng0007/article/details/107066856#private_165)
- [访问非private类方法](https://blog.csdn.net/ShuSheng0007/article/details/107066856#private_174)
- [访问非private属性](https://blog.csdn.net/ShuSheng0007/article/details/107066856#private_183)
- [访问private属性](https://blog.csdn.net/ShuSheng0007/article/details/107066856#private_190)
- [增强MethodHandle](https://blog.csdn.net/ShuSheng0007/article/details/107066856#MethodHandle_199)



## 3、MethodHandle使用

1. 创建MethodType
2. 创建Lookup
3. 基于Lookup与MethodType获得MethodHandle
4. 调用MethodHandle