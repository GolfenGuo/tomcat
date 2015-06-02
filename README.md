# Tomcat

镜像“Tomcat”源自DockerHub镜像[tutum/Tomcat](https://registry.hub.docker.com/u/tutum/tomcat/)

## 版本

当前版本 Tomcat 7.0.55

## 说明

容器启动后会自动创建一个具有所有权限的admin用户，并自动生成随机密码。你可以通过查看容器日志获得密码，比如

> ========================================================================
> You can now connect to this Tomcat server using:
> 
>     admin:b1uKcRK3r6SF
> 
> Please remember to change the above password as soon as possible!
> 
> ========================================================================

在上面的例子中，*b1uKcRK3r6SF* 就是admin用户的密码。

你可以用admin用户访问下面的地址配置Tomcat:

－ http://your-tomcat-url/manager/html
－ http://your-tomcat-url/host-manager/html

如果你想为admin用户设置一个特定的密码，你可以设置环境变量 *TOMCAT_PASS* 为您需要的密码。


