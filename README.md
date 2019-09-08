# tomcat6_images
eg:  
```
docker build -f ./tomcat-6.0.53/dockerfile -t tocmat:6.53 ./tomcat-6.0.53/
simple example:
docker run -itd tocmat:6.53
complete example:
docker run -itd  -v logs:/usr/local/tomcat/logs -v conf/server.xml:/usr/local/tomcat/conf/server.xml -v webapps:/usr/local/tomcat/webapps --name tocmat tocmat:6.53
```
**注意:dockerfile里需要通外网yum安装一些依赖包,增加代理方法ENV http_proxy="http://xxxx"**
