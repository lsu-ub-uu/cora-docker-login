ARG CORA_DOCKER_VERSION
FROM cora-docker-tomcat:${CORA_DOCKER_VERSION}

COPY /cora-login-war*.war /usr/local/tomcat/webapps/login.war
COPY /login.xml /usr/local/tomcat/conf/Catalina/localhost/login.xml