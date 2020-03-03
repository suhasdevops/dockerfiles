FROM ubuntu:18.04

MAINTAINER suhasdevops

RUN apt-get -y update && apt-get -y upgrade
RUN apt-get -y install openjdk-8-jre-headless
RUN apt-get -y install wget

WORKDIR /opt/
RUN wget http://apache.cbox.biz/tomcat/tomcat-9/v9.0.31/bin/apache-tomcat-9.0.31.tar.gz
RUN tar -zvxf apache-tomcat-9.0.31.tar.gz

EXPOSE 8080
CMD bash /opt/apache-tomcat-9.0.31/bin/startup.sh


# copy above code in Dockerfile and run below commands:

# to buils an docke image
# $ docker build -t <imagename> .

# $ docker images

# to run docker image
# $ docker run -dit -p 8080:8080 <imagename> /bin/bash

# $ docker ps

# to open docker container's cmd prompt
# $ docker exec -it <container id> /bin/bash

# check with browser tomcat page is open/not, if tomcat is not open restart the tomcat service on container... :)