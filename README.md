# tomcat 9.0 run Alpine Linx with openjdk8



### tomcat安装路径

/usr/local/tomcat



### 默认站点目录

/usr/local/tomcat/webapps/ROOT



### 默认工作目录

/usr/local/tomcat/webapps



### tomcat9 配置文件目录

/usr/local/tomcat/conf



### JAVA_HOME 路径

/usr/lib/jvm/default-jvm



PATH

/usr/lib/jvm/default-jvm/bin



配置为官方默认配置，如果需要自定义配置，在容器运行的时候指定你本地配置文件路径后 持久化到容器对应的目录或则文件即可

如使用自定义的配置文件 server.xml， 则准备好server.xml配置文件，然后运行容器 

~~~shell
docker run -it -d --name tomcat9 -p 8080:8080  -v /localpath/server.xml:/usr/local/tomcat/conf/server.xml  tekintian/alpine-tomcat:9.0
~~~



Tomcat9官方网站

https://tomcat.apache.org/tomcat-9.0-doc/index.html





| Package     | openjdk8                                                     |
| ----------- | ------------------------------------------------------------ |
| Version     | **8.181.13-r0**                                              |
| Description | OpenJDK 8 provided by IcedTea                                |
| Project     | <https://icedtea.classpath.org/>                             |
| Contents    | [Openjdk8 Contents of package](https://pkgs.alpinelinux.org/contents?branch=edge&name=openjdk8&arch=s390x&repo=community) |



TekinTian

tekintian@gmail.com





