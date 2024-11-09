FROM tomcat:11.0.0-jdk11

RUN apt-get update && apt-get -y upgrade

COPY ../../build/libs/internship_project.war /usr/local/tomcat/webapps/

EXPOSE 8080

CMD ["catalina.sh", "run"]
