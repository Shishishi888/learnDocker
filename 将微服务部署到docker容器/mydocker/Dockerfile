FROM java:8
# 作者
MAINTAINER ShiYang
# VOLUME 指定临时文件目录为/tmp，在主机/var/lib/docker目录下创建了一个临时文件并链接到容器的/tmp
VOLUME /tmp
# 将jar包添加到容器中并更名为zzyy_docker.jar
ADD DockerRoot-0.0.1-SNAPSHOT.jar shiyang_docker.jar
# 运行jar包
RUN bash -c 'touch /zzyy_docker.jar'
ENTRYPOINT ["java","-jar","/shiyang_docker.jar"]
#暴露6001端口作为微服务
EXPOSE 6001
