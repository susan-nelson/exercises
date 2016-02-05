HOW TO BUILD and RUN:
====================
This project depends on an installation of the following:
    for build, maven 3
        see maven.apache.org
    to run, java 8
        see oracle.com/technetwork/java/javase/downloads/index.html

To build and startup with embedded tomcat:
    cd  to root of project
    mvn clean spring-boot:run

To exit:
    ctrl-c

To create an executable jar:
    cd  to root of project
    mvn clean package
    (creates soap-webservices-0.0.1-SNAPSHOT.jar)

To execute jar from the command line at root of project:
    java -jar target/soap-webservices-0.0.1-SNAPSHOT.jar

To test:
cd to project root
curl --header "content-type: text/xml" -d @src/test/resourses/request.xml http://localhost:8080/ws


