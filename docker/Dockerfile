ARG CORA_DOCKER_VERSION
FROM cora-docker-tomcat:${CORA_DOCKER_VERSION}

COPY /cora-apptokenverifier-war*.war /usr/local/tomcat/webapps/apptokenverifier.war
COPY /apptokenverifier.xml /usr/local/tomcat/conf/Catalina/localhost/apptokenverifier.xml