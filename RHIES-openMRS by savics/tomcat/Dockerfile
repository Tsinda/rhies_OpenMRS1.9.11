FROM openjdk:7

RUN curl -o /opt/tomcat7.tar.gz https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.79/bin/apache-tomcat-7.0.79.tar.gz
RUN tar -xzf /opt/tomcat7.tar.gz -C /root/ --strip-components=1
RUN rm -f /opt/tomcat7.tar.gz
ADD http://www.datanucleus.org/downloads/maven2/oracle/ojdbc6/11.2.0.3/ojdbc6-11.2.0.3.jar /root/lib
COPY tomcat-users.xml /root/conf/
COPY run.sh /root/bin/
RUN sed -i.bak 's/HTTP\/1\.1"/HTTP\/1\.1" URIEncoding="UTF-8"/g' /root/conf/server.xml




ADD openmrs-runtime.properties /root/openmrs-runtime.properties
ADD modules/ /root/.OpenMRS/modules/
ADD setenv.sh /root/bin/setenv.sh
ADD openmrs.war /root/webapps/openmrs.war

EXPOSE 8080

CMD ["/root/bin/run.sh"]
