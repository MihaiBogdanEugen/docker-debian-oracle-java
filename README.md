## Docker Debian images with [Oracle Java] (JDK/JRE/ServerJRE) ##

### Supported tags and respective Dockerfile links: ###

* ```jessie-slim-jdk8``` _\([jessie-slim-jdk8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-jdk8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-jdk8 "")
* ```jessie-slim-jre8``` _\([jessie-slim-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-jre8 "")
* ```jessie-slim-server-jre8``` _\([jessie-slim-server-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-server-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-server-jre8 "")
* ```jessie-slim-jdk11``` _\([jessie-slim-jdk11/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-jdk11.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-jdk11 "")
* ```stretch-slim-jdk8``` _\([stretch-slim-jdk8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-jdk8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-jdk8 "")
* ```stretch-slim-jre8``` _\([stretch-slim-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-jre8 "")
* ```stretch-slim-server-jre8``` _\([stretch-slim-server-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-server-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-server-jre8 "")
* ```stretch-slim-jdk11```, ```latest``` _\([stretch-slim-jdk11/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-jdk11.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-jdk11 "")

#### All tag names follow the naming convention: ###

```debian_image_tag``` + '-' + ```jdk/jre/server-jre``` + ```java_version```

### Usage: ###

Build the image
```shell
docker build -t mbe1224/debian-oracle-java /stretch-slim/java11/jdk/
```

### About this image: ###

- Currently supporting java versions **8u192** and **11.0.1**
- Debian "slim" image variant
- Oracle Java (JDK/JRE/ServerJRE) addded without MissionControl, VisualVM, JavaFX, ReadMe files, source archives, etc.
- Oracle Java Cryptography Extension added
- SHA 256 sum checks for all downloads
- JAVA\_HOME environment variable set up

### Dual licensed under: ###

* [MIT License]
* [Oracle Binary Code License Agreement]

   [Oracle Java]: <http://www.oracle.com/technetwork/java/javase/downloads/index.html>
   [jessie-slim-jdk8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java8/jdk/Dockerfile>
   [jessie-slim-jre8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java8/jre/Dockerfile>
   [jessie-slim-server-jre8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java8/server-jre/Dockerfile>  
   [jessie-slim-jdk11/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java11/jdk/Dockerfile>
   [stretch-slim-jdk8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/jdk/Dockerfile>
   [stretch-slim-jre8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/jre/Dockerfile>
   [stretch-slim-server-jre8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/server-jre/Dockerfile>
   [stretch-slim-jdk11/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java11/jdk/Dockerfile>
   [MIT License]: <https://raw.githubusercontent.com/MihaiBogdanEugen/docker-debian-oracle-java/master/LICENSE>
   [Oracle Binary Code License Agreement]: <https://raw.githubusercontent.com/MihaiBogdanEugen/docker-debian-oracle-java/master/Oracle_Binary_Code_License_Agreement%20for%20the%20Java%20SE%20Platform_Products_and_JavaFX>
