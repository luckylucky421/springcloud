FROM java:8-jdk-alpine
RUN  apk add -U tzdata && \
     ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
COPY ./target/eureka-service.jar ./
EXPOSE 8888
CMD java -jar -Deureka.instance.hostname=${MY_POD_NAME}.eureka.ms /eureka-service.jar
