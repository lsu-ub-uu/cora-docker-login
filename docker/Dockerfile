ARG CORA_DOCKER_VERSION
FROM cora-docker-tomcat:${CORA_DOCKER_VERSION}


COPY /apptokenverifier*.war /usr/local/tomcat/webapps/apptokenverifier.war
COPY /apptokenverifier.xml /usr/local/tomcat/conf/Catalina/localhost/apptokenverifier.xml

COPY /*.jar /usr/local/tomcat/lib/
#COPY /*.properties /usr/local/tomcat/lib/

#build with:
#maven build

#start on development with:
#docker run --net=cora --volumes-from gatekeeper:ro -p 8082:8080 --name apptokenverifier --link gatekeeper:gatekeeper -d  apptokenverifier


#start on build server with:
#docker run --net=cora-test --volumes-from gatekeeper-test --name apptokenverifier-test --link gatekeeper-test:gatekeeper -d  apptokenverifier

#start on external with:
#docker run --network=cora --name apptokenverifier --link gatekeeper:gatekeeper -d  apptokenverifier
