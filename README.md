# Tomcat

镜像“Tomcat”源自DockerHub镜像[tutum/Tomcat](https://registry.hub.docker.com/u/tutum/tomcat/)。

## 版本

当前版本 Tomcat 7.0.55

## 说明

容器启动后会自动创建一个具有所有权限的admin用户，并自动生成随机密码。你可以通过查看容器log获得密码，比如

> => Creating and admin user with a random password in Tomcat
> 
> ========================================================================
> 
>       admin : tTUFq9xLDlpc

在上面的例子中，*tTUFq9xLDlpc* 就是admin用户的密码。

你可以用admin用户访问下面的地址配置Tomcat:

－ http://your-tomcat-url/manager/html
－ http://your-tomcat-url/host-manager/html

如果你想为admin用户设置一个特定的密码，你可以设置环境变量 *TOMCAT_PASS* 为您需要的密码。


