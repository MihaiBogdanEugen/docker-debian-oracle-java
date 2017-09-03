## Debian Docker image with Oracle JDK

### Supported tags and respective Dockerfile links:

* ```jesse-slim-8u144``` _\([jesse-slim-8u144/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oraclejdk:jesse-slim-8u144.svg)](https://microbadger.com/images/mbe1224/debian-oraclejdk:jesse-slim-8u144 "")
* ```stretch-slim-8u144``` _\([stretch-slim-8u144/Dockerfile]\)_
[![](https://images.microbadger.com/badges/image/mbe1224/debian-oraclejdk:jstretch-slim-8u144.svg)](https://microbadger.com/images/mbe1224/debian-oraclejdk:stretch-slim-8u144 "")

#### All tag names follow the naming convention:

```debian_image_tag``` + '-' + ```java_version```

### Usage:

Build the image
```shell
docker build -t mbe1224/debian-oraclejdk .
```

### About this image:

- Debian "slim" image variant
- Oracle Java SE Development Kit (JDK) addded, without MissionControl, VisualVM, JavaFX and JRE
- Oracle Java Cryptography Extension added
- SHA 256 sum checks for all downloads
- JAVA\_HOME environment variable set up

### License:

* [MIT License]
* [Oracle Binary Code License Agreement]

   [jesse-slim-8u144/Dockerfile]: <https://github.com/MihaiBogdanEugen/debian-oraclejdk/blob/jesse-slim-8u144/Dockerfile>
   [stretch-slim-8u144/Dockerfile]: <https://github.com/MihaiBogdanEugen/debian-oraclejdk/blob/stretch-slim-8u144/Dockerfile>
   [MIT License]: <https://raw.githubusercontent.com/MihaiBogdanEugen/debian-oraclejdk/master/LICENSE>
   [Oracle Binary Code License Agreement]: <https://raw.githubusercontent.com/MihaiBogdanEugen/debian-oraclejdk/master/Oracle_Binary_Code_License_Agreement%20for%20the%20Java%20SE%20Platform_Products_and_JavaFX>