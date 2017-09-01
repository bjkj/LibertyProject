## Liberty App Accelerator
This project was generated by the [Liberty app accelerator](http://ibm.biz/appaccelerator)

[![](https://img.shields.io/badge/bluemix-powered-blue.svg)](https://bluemix.net)
[![Platform](https://img.shields.io/badge/platform-java-lightgrey.svg?style=flat)](https://www.ibm.com/developerworks/learn/java/)

### Table of Contents
* [Summary](#summary)
* [Requirements](#requirements)
* [Configuration](#configuration)
* [Project contents](#project-contents)
* [Run](#run)
* [Notices](#notices)

### Summary

The Liberty App Accelerator provides a starting point for creating applications running on [WebSphere Liberty](https://developer.ibm.com/wasdev/).


### Requirements
* [Maven](https://maven.apache.org/install.html)
* Java 8: Any compliant JVM should work.
  * [Java 8 JDK from Oracle](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
  * [Java 8 JDK from IBM (AIX, Linux, z/OS, IBM i)](http://www.ibm.com/developerworks/java/jdk/),
    or [Download a Liberty server package](https://developer.ibm.com/assets/wasdev/#filter/assetTypeFilters=PRODUCT)
    that contains the IBM JDK (Windows, Linux)

### Configuration
The application is configured to provide various technologies and features. These capabilities are provided through dependencies in the pom.xml file and Liberty features enabled in the server config file found in `src/main/liberty/config/server.xml`.

### Project contents
The context root is set in the `src/main/webapp/WEB-INF/ibm-web-ext.xml` file. The ports are set in the pom.xml file.      

* **Swagger** : Swagger is a simple yet powerful representation of RESTful APIs. Discover REST APIs that are available on the Liberty server and then invoke the found REST endpoints using the Swagger user interface. (Username and password are specified in the server.xml). You can also easily expose the REST endpoints available from your web modules running on Liberty server by documenting the endpoints using the Swagger 2.0 Specification. It is also possible to follow a design-first approach by creating the Swagger documentation first and then generating the server code from it. For the complete feature documentation, see the [apiDiscovery-1.0](http://www.ibm.com/support/knowledgecenter/en/SSEQTP_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/rwlp_feature_apiDiscovery-1.0.html) feature description in IBM Knowledge Center.    
### Run

To build and run the application:
1. `mvn install`
1. `mvn liberty:run-server`
 

### Endpoints

The context root is set in the `src/main/webapp/WEB-INF/ibm-web-ext.xml` file. The ports are set in the pom.xml file.

### Notices

This project was generated using:
* generator-java v2.2.1
* java-common v2.2.0
* generator-ibm-service-enablement v^0.0.59
* generator-ibm-cloud-enablement v^0.0.68
* generator-liberty v5.2.0
