## Docker Debian images with Oracle Java (JDK/JRE/ServerJRE)

### Supported tags and respective Dockerfile links:

* ```jessie-slim-jdk-8u152```, ```jessie-slim-jdk8-latest``` _\([jessie-slim-jdk-8u152/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:jessie-slim-jdk-8u152.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:jessie-slim-jdk-8u152 "")
* ```jessie-slim-jre-8u152```, ```jessie-slim-jre8-latest``` _\([jessie-slim-jre-8u152/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:jessie-slim-jre-8u152.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:jessie-slim-jre-8u152 "")
* ```jessie-slim-server-jre-8u152```, ```jessie-slim-server-jre8-latest``` _\([jessie-slim-server-jre-8u152/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:jessie-slim-server-jre-8u152.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:jessie-slim-server-jre-8u152 "")
* ```jessie-slim-jdk-9.0.1```, ```jessie-slim-jdk9-latest``` _\([jessie-slim-jdk-9.0.1/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:jessie-slim-jdk-9.0.1.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:jessie-slim-jdk-9.0.1 "")
* ```jessie-slim-jre-9.0.1```, ```jessie-slim-jre9-latest``` _\([jessie-slim-jre-9.0.1/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:jessie-slim-jre-9.0.1.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:jessie-slim-jre-9.0.1 "")
* ```jessie-slim-server-jre-9.0.1```, ```jessie-slim-server-jre9-latest``` _\([jessie-slim-server-jre-9.0.1/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:jessie-slim-server-jre-9.0.1.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:jessie-slim-server-jre-9.0.1 "")
* ```stretch-slim-jdk-8u152```, ```stretch-slim-jdk8-latest``` _\([stretch-slim-jdk-8u152/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:stretch-slim-jdk-8u152.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:stretch-slim-jdk-8u152 "")
* ```stretch-slim-jre-8u152```, ```stretch-slim-jre8-latest``` _\([stretch-slim-jre-8u152/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:stretch-slim-jre-8u152.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:stretch-slim-jre-8u152 "")
* ```stretch-slim-server-jre-8u152```, ```stretch-slim-server-jre8-latest``` _\([stretch-slim-server-jre-8u152/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:stretch-slim-server-jre-8u152.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:stretch-slim-server-jre-8u152 "")
* ```stretch-slim-jdk-9.0.1```, ```stretch-slim-jdk9-latest``` _\([stretch-slim-jdk-9.0.1/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:stretch-slim-jdk-9.0.1.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:stretch-slim-jdk-9.0.1 "")
* ```stretch-slim-jre-9.0.1```, ```stretch-slim-jre9-latest```, ```latest``` _\([stretch-slim-jre-9.0.1/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:stretch-slim-jre-9.0.1.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:stretch-slim-jre-9.0.1 "")
* ```stretch-slim-server-jre-9.0.1```, ```stretch-slim-server-jre9-latest``` _\([stretch-slim-server-jre-9.0.1/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/docker-debian-oracle-java:stretch-slim-server-jre-9.0.1.svg)](https://microbadger.com/images/mbe1224/docker-debian-oracle-java:stretch-slim-server-jre-9.0.1 "")

#### All tag names follow the naming convention:

```debian_image_tag``` + '-' + ```jdk/jre/server-jre``` + '-' + ```java_version```

### Usage:

Build the image
```shell
docker build -t mbe1224/debian-oraclejdk .
```

### About this image:

- Debian "slim" image variant
- Oracle Java (JDK/JRE/ServerJRE) addded without MissionControl, VisualVM, JavaFX, ReadMe files, source archives, etc.
- Oracle Java Cryptography Extension added
- SHA 256 sum checks for all downloads
- JAVA\_HOME environment variable set up

### License:

* [MIT License]
* [Oracle Binary Code License Agreement]

   [jessie-slim-jdk-8u152/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java8/jdk/Dockerfile>
   [jessie-slim-jre-8u152/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java8/jre/Dockerfile>
   [jessie-slim-server-jre-8u152/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java8/server-jre/Dockerfile>  
   [jessie-slim-jdk-9.0.1/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java9/jdk/Dockerfile>
   [jessie-slim-jre-9.0.1/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java9/jre/Dockerfile>
   [jessie-slim-server-jre-9.0.1/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/jessie-slim/java9/server-jre/Dockerfile>  
   [stretch-slim-jdk-8u152/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/jdk/Dockerfile>
   [stretch-slim-jre-8u152/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/jre/Dockerfile>
   [stretch-slim-server-jre-8u152/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java8/server-jre/Dockerfile>  
   [stretch-slim-jdk-9.0.1/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java9/jdk/Dockerfile>
   [stretch-slim-jre-9.0.1/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java9/jre/Dockerfile>
   [stretch-slim-server-jre-9.0.1/Dockerfile]: <https://github.com/MihaiBogdanEugen/docker-debian-oracle-java/blob/master/stretch-slim/java9/server-jre/Dockerfile>
   [MIT License]: <https://raw.githubusercontent.com/MihaiBogdanEugen/debian-oraclejdk/master/LICENSE>
   [Oracle Binary Code License Agreement]: <https://raw.githubusercontent.com/MihaiBogdanEugen/debian-oraclejdk/master/Oracle_Binary_Code_License_Agreement%20for%20the%20Java%20SE%20Platform_Products_and_JavaFX>