## Docker Debian images with [Oracle Java] (JDK/JRE/ServerJRE) ##

### Supported tags and respective Dockerfile links: ###

* ```jessie-slim-jdk8``` _\([jessie-slim-jdk8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-jdk8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-jdk8 "")
* ```jessie-slim-jre8``` _\([jessie-slim-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-jre8 "")
* ```jessie-slim-server-jre8``` _\([jessie-slim-server-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-server-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-server-jre8 "")
* ```jessie-slim-jdk9``` _\([jessie-slim-jdk9/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-jdk9.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-jdk9 "")
* ```jessie-slim-jre9``` _\([jessie-slim-jre9/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-jre9.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-jre9 "")
* ```jessie-slim-server-jre9``` _\([jessie-slim-server-jre9/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:jessie-slim-server-jre9.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:jessie-slim-server-jre9 "")
* ```stretch-slim-jdk8``` _\([stretch-slim-jdk8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-jdk8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-jdk8 "")
* ```stretch-slim-jre8``` _\([stretch-slim-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-jre8 "")
* ```stretch-slim-server-jre8``` _\([stretch-slim-server-jre8/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-server-jre8.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-server-jre8 "")
* ```stretch-slim-jdk9```, ```latest``` _\([stretch-slim-jdk9/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-jdk9.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-jdk9 "")
* ```stretch-slim-jre9``` _\([stretch-slim-jre9/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-jre9.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-jre9 "")
* ```stretch-slim-server-jre9``` _\([stretch-slim-server-jre9/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oracle-java:stretch-slim-server-jre9.svg)](https://microbadger.com/images/mbe1224/debian-oracle-java:stretch-slim-server-jre9 "")

#### All tag names follow the naming convention: ###

```debian_image_tag``` + '-' + ```jdk/jre/server-jre``` + ```java_version```

### Usage: ###

Build the image
```shell
docker build -t mbe1224/debian-oracle-java /stretch-slim/java9/jdk/
```

### About this image: ###

- Currently supporting java versions **8u152** and **9.0.1**
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
   [jessie-slim-jdk9/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java9/jdk/Dockerfile>
   [jessie-slim-jre9/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java9/jre/Dockerfile>
   [jessie-slim-server-jre9/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java9/server-jre/Dockerfile>  
   [stretch-slim-jdk8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/jdk/Dockerfile>
   [stretch-slim-jre8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/jre/Dockerfile>
   [stretch-slim-server-jre8/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/server-jre/Dockerfile>
   [stretch-slim-jdk9/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java9/jdk/Dockerfile>
   [stretch-slim-jre9/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java9/jre/Dockerfile>
   [stretch-slim-server-jre9/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java9/server-jre/Dockerfile> 
   [MIT License]: <https://raw.githubusercontent.com/MihaiBogdanEugen/docker-debian-oracle-java/master/LICENSE>
   [Oracle Binary Code License Agreement]: <https://raw.githubusercontent.com/MihaiBogdanEugen/docker-debian-oracle-java/master/Oracle_Binary_Code_License_Agreement%20for%20the%20Java%20SE%20Platform_Products_and_JavaFX>