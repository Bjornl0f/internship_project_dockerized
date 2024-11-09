FROM openjdk:11-jre-slim

RUN apt-get update && apt-get install -y wget

RUN wget https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/apache-tomcat-9.0.50.tar.gz && \
    tar xvf apache-tomcat-9.0.50.tar.gz && \
    mv apache-tomcat-9.0.50 /usr/local/tomcat

COPY build/libs/class_schedule.war /usr/local/tomcat/webapps/

EXPOSE 8080

CMD ["/usr/local/tomcat/bin/catalina.sh", "run"]
