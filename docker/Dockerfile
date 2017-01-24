FROM  tomcat:jre8-alpine

COPY /storagefiles /mnt/data/basicstorage

COPY /apptokenverifier.war /usr/local/tomcat/webapps/apptokenverifier.war
COPY /apptokenverifier.xml /usr/local/tomcat/conf/Catalina/localhost/apptokenverifier.xml
COPY /basicstorage.jar /usr/local/tomcat/lib/basicstorage.jar
#build with maven build


#build with:
#maven build

#start on development with:
#docker run --net=cora -p 8082:8080 --name apptokenverifier --link gatekeeper:gatekeeper -d  apptokenverifier

#start on build server with:
#docker run --network=cora-test --name apptokenverifier-test --link gatekeeper:gatekeeper -d  apptokenverifier

#start on external with:
#docker run --network=cora --name apptokenverifier --link gatekeeper:gatekeeper -d  apptokenverifier
