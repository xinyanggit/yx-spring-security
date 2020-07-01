代码是对着公众号 松哥笔记学习的
1、添加对应的pom之后，所有的资源全部都被管理了。
访问都会被跳转到login 页面
控制台的输出就是密码。
1、配置文件配置用户密码
配置application.properties 的文件
java体现中
@ConfigurationProperties(prefix = "spring.security")
org.springframework.boot.autoconfigure.security.SecurityProperties
2、java代码中配置
 详细介绍可以看com.yx.security.config.CustomerSecurityConfig
 一些配置都在代码中解释了
3、自定义表单登录
com.yx.security.config.CustomerSecurityConfig 查看
4、前后端分离 json交互
  jwt 和session(自动续签，当时移动端，小程序不支持cookie,session 就有弊端)
  无状态登录和有状态登录
 目前都是session 
登陆成功 登录失败 无权限访问的回调函数解释
 
5、角色的继承关系
