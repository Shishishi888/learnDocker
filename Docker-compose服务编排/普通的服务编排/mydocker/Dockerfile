# 基础镜像使用java
FROM java:8
# 作者
MAINTAINER shiyang
# VOLUME 指定临时文件目录为/tmp，在主机/var/lib/docker目录下创建了一个临时文件并链接到容器的/tmp
VOLUME /tmp
# 将jar包添加到容器中并更名为shiyang_docker.jar
ADD DockerBoot-0.0.1-SNAPSHOT.jar shiyang_docker.jar
# 运行jar包
RUN bash -c 'touch /shiyang_docker.jar'
ENTRYPOINT ["java","-jar","/shiyang_docker.jar"]
#暴露6001端口作为微服务
EXPOSE 6001
