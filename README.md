#Spring Boot - Eureka Server

# App Name : discovery-server
A Demo project for spring-cloud-netflix Eureka Server.

In my repo each spring boot application is a Micro service will register into the Eureka server and Eureka server knows all the client applications running on each port and IP address. Eureka Server is also known as Discovery Server.

#Build : 
Open with any ide and use Maven, use the command − mvn clean install

#just want properties here are the details please copy and add into your yml file.

server:
  port: 8761 #default port where discovery client is registered

eureka:
  client:
    eurekaServerConnectTimeoutSeconds: 5
    enabled: true
    registerWithEureka: false
    fetchRegistry: false
  server:
    waitTimeInMsWhenSyncEmpty: 0
    
