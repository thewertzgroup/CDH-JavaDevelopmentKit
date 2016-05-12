# CDH-JavaDevelopmentKit

http://www.cloudera.com/documentation/enterprise/latest/topics/cdh_ig_jdk_installation.html

## Installing the Oracle JDK

The Oracle JDK installer is available both as an RPM-based installer for RPM-based systems, and as a binary installer for other systems.

1. Download the .tar.gz file for one of the supported versions of the Oracle JDK from Java SE 8 Downloads or Java SE 7 Downloads. (These links are correct at the time of writing but change frequently.)
2. Extract the JDK to /usr/java/jdk-version; for example /usr/java/jdk.1.7.0_nn or /usr/java/jdk.1.8.0_nn, where nn is a supported version.
3. Set JAVA_HOME to the directory where the JDK is installed, for example
  ```
  export JAVA_HOME=/usr/java/jdk.1.7.0_nn
  ```
in the following files on Cloudera Manager Server and cluster hosts:
  * Cloudera Manager Server - /etc/default/cloudera-scm-server. This change affects only the Cloudera Manager Server process, and does not affect the Cloudera Management Service roles.
  * Cloudera Manager package-based or unmanaged deployment - /etc/default/bigtop-utils

4. Follow the instructions in Configuring a Custom Java Home Location. This change affects all CDH processes and Cloudera Management Service roles in the cluster.

http://www.cloudera.com/documentation/enterprise/latest/topics/cm_ig_java_home_location.html
