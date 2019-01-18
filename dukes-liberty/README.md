
### Table of Contents
* [Summary](#summary)
* [Requirements](#requirements)
* [Configuration](#configuration)
* [Project contents](#project-contents)
* [Run](#run)
* [Notices](#notices)

### Summary

The dukes-liberty application provides simple examples demonstrating various features of the [MicroProifle](https://microprofile.io) programming model using the [Open Liberty](https://openliberty.io) application server.

### Requirements
* [Maven](https://maven.apache.org/install.html)
* Java 8: Any compliant JDK should work.
  * [Java 8 JDK from Oracle](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
  * [Java 8 JDK from IBM (AIX, Linux, z/OS, IBM i)](http://www.ibm.com/developerworks/java/jdk/)
  * [AdoptOpenJDK 8 (OpenJ9 or Hotspot JVM)](https://adoptopenjdk.net/index.html)

### Configuration
The application is configured to provide various technologies and features. These capabilities are provided through dependencies in the pom.xml file and Open Liberty features enabled in the server config file found in `src/main/liberty/config/server.xml`.

### Project contents
The context root (dukes-liberty) is set in the `src/main/webapp/WEB-INF/ibm-web-ext.xml` file. The ports are set in the pom.xml file.

* **MicroProfile** : The [MicroProfile project](http://microprofile.io/) is an open community with the aim of optimizing Enterprise Java for a microservices architecture.  MicroProfile will be evolving with guidance from the community. For the complete feature documentation, see the [MicroProfile programming model section](https://www.ibm.com/support/knowledgecenter/SSEQTP_liberty/com.ibm.websphere.wlp.doc/ae/rwlp_microprofile.html) in the IBM Knowledge Center. Or, for more hands-on MicroProfile learning, check out the [Open Liberty Guides](https://openliberty.io/guides/?search=microprofile).  If you want to share your thoughts you can post straight to the [MicroProfile Google group](https://groups.google.com/forum/#!forum/microprofile).  

### Run

To build and run the application:
1. `mvn clean install`
1. `mvn liberty:run-server`  (ctrl-c ends the server)

* Dukes-Liberty Endpoint:  http://localhost:9080/dukes-liberty
* MicroProfile Health Endpoint:  http://localhost:9080/health
* OpenAPI UI:  http://localhost:9080/openapi/ui/
* Health API Endpoint:  http://localhost:9080/dukes-liberty/api/health
* Hello API Endpoint:  http://localhost:9080/dukes-liberty/api/hello

### Endpoints

The context root (dukes-liberty) is set in the `src/main/webapp/WEB-INF/ibm-web-ext.xml` file. The ports are set in the pom.xml file.
