#基础镜像
FROM zengxiangkai/jdk8:centos7
#作者
LABEL maintainer="14268414+Thousandcherry@users.noreply.github.com"
#创建目录
RUN mkdir /opt/app
#编译镜像时复制maven package打包生成的jar到镜像对应的目录下
COPY eureka-server-0.0.1-SNAPSHOT.jar /opt/app
#开放端口
EXPOSE 3000
#启动时执行的命令，这里还可以添加jar启动环境变量参数
ENTRYPOINT ["java","-jar","/opt/app/eureka-server-0.0.1-SNAPSHOT.jar"]