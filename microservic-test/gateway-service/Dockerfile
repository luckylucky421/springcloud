FROM java:8-jdk-alpine
RUN  apk add -U tzdata && \
     ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
COPY ./target/gateway-service.jar ./
EXPOSE 9999
CMD java -jar /gateway-service.jar
