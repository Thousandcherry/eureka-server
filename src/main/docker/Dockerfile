#基础镜像
FROM adoptopenjdk/openjdk8:centos
#作者
LABEL maintainer="14268414+Thousandcherry@users.noreply.github.com"
RUN mkdir /opt/app
#编译镜像时复制maven package打包生成的jar到镜像中
COPY eureka-server-0.0.1-SNAPSHOT.jar /opt/app
#开放端口
EXPOSE 3000
#启动时执行的命令
ENTRYPOINT ["java","-jar","/usr/local/eureka-server-0.0.1-SNAPSHOT.jar"]