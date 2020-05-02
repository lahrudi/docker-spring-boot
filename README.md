# Read Me First
The following was discovered as part of building this project:
1.Create simple spring boot application.
2.How to create docker image and run spring boot application in docker engine.
* The original package name 'com.docker' is invalid and this project uses 'com.docker' instead.

# Getting Started
* Create project in with `https://start.spring.io` .
* Config server port.
* Run maven `clean install` command to build application.
* Open terminal window and run this command: `docker build -f DockerFile -t docker-spring-boot .` .
* Assign favorite port to specified port in application.properties file with this command :
    `docker run -p [favorite port]:[expose or open specified port in application.properties] [application name]`
    example : docker run -p 8085:8080 docker-spring-boot
    The app will run on port 80. By default, you won’t be able to access the web app on port 8080 from your host machine. You will have to tell Docker that you want to expose or open port 8080 to be able to access it from your host machine.    
### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.2.6.RELEASE/maven-plugin/)

