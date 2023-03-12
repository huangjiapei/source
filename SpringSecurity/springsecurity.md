### 1、认证

#### 1.1 登录校验流程   

![认证](.\image\认证.png)

#### 1.2 springSecurity完整流程

![完整流程](.\image\完整流程.png)

#### 1.3 认证原理

![认证原理](.\image\认证原理.png)

![信息](.\image\信息.png)

#### 1.4 自定义认证逻辑

最简单方法：重新配置认证服务



![认证思路](.\image\认证思路.png)

![自定义认证逻辑](.\image\自定义认证逻辑.png)

![jwt过滤器](.\image\jwt过滤器.png)



#### 1.5 配置

https://blog.csdn.net/m0_51945027/article/details/119568320

https://ximeneschen.blog.csdn.net/article/details/123977133?spm=1001.2101.3001.6661.1&utm_medium=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-123977133-blog-104573094.pc_relevant_multi_platform_whitelistv3&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-1-123977133-blog-104573094.pc_relevant_multi_platform_whitelistv3&utm_relevant_index=1

https://blog.csdn.net/a2231476020/article/details/99735222

https://www.jianshu.com/p/641aebc58682

【认证、授权配置】https://blog.csdn.net/qq_53609683/article/details/121050306

##### （1）编写认证、权限逻辑

![权限代码](D:\Environment\GitSpace\future\source\source\SpringSecurity\image\权限代码.png)

##### （2）配置认证、授权

AuthenticationManagerBuilder【认证】、HttpSecurity【授权】

![常用配置](\image\常用配置.png)

##### （3）配置WebSecurity

![](.\image\配置httpsecurity.png)

![配置](\image\配置.png)
