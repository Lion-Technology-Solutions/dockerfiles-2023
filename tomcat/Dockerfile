FROM tomcat
RUN mkdir /opt/tomcat/
WORKDIR /opt/tomcat
ADD  https://dlcdn.apache.org/tomcat/tomcat-10/v10.0.27/bin/apache-tomcat-10.0.27.tar.gz .
RUN tar xvfz apache*.tar.gz \
&& mv apache-tomcat-10.0.27/* /opt/tomcat/. \
&& apt-get -y update \
&& apt-get install openjdk-8-jdk -y \
&& java --version
WORKDIR /opt/tomcat/webapps
EXPOSE 8080
CMD ["/opt/tomcat/bin/catalina.sh", "run"]