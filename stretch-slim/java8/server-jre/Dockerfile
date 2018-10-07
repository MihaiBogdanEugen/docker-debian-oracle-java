# Start from debian stretch-slim
FROM debian:stretch-slim

# Setup JAVA_HOME
ENV JAVA_HOME="/usr/lib/jvm/default-jvm"

# Install Oracle Server JRE (Java SE Runtime Environment) 8u171 with Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy Files for JDK/JRE 8
RUN JAVA_VERSION=8 && \
    JAVA_UPDATE=171 && \
    JAVA_BUILD=13 && \
    JAVA_PATH=96a7b8442fe848ef90c96a2fad6ed6d1 && \
    JAVA_SHA256_SUM=678e798008c398be98ba9d39d5114a9b4151f9d3023ccdce8b56f94c5d450698 && \
    JCE_SHA256_SUM=f3020a3922efd6626c2fff45695d527f34a8020e938a49292561f18ad1320b59 && \ 
    apt-get update && \
    apt-get -y install wget unzip && \
    cd "/tmp" && \
    wget --header "Cookie: oraclelicense=accept-securebackup-cookie;" "http://download.oracle.com/otn-pub/java/jdk/${JAVA_VERSION}u${JAVA_UPDATE}-b${JAVA_BUILD}/${JAVA_PATH}/server-jre-${JAVA_VERSION}u${JAVA_UPDATE}-linux-x64.tar.gz" && \
    echo "${JAVA_SHA256_SUM}" "server-jre-${JAVA_VERSION}u${JAVA_UPDATE}-linux-x64.tar.gz" | sha256sum -c - && \
    wget --header "Cookie: oraclelicense=accept-securebackup-cookie;" "http://download.oracle.com/otn-pub/java/jce/${JAVA_VERSION}/jce_policy-${JAVA_VERSION}.zip" && \
    echo "${JCE_SHA256_SUM}" "jce_policy-${JAVA_VERSION}.zip" | sha256sum -c - && \
    tar -xzf "server-jre-${JAVA_VERSION}u${JAVA_UPDATE}-linux-x64.tar.gz" && \
    mkdir -p "/usr/lib/jvm" && \
    mv "/tmp/jdk1.${JAVA_VERSION}.0_${JAVA_UPDATE}" "/usr/lib/jvm/java-${JAVA_VERSION}-oracle" && \
    ln -s "java-${JAVA_VERSION}-oracle" "$JAVA_HOME" && \
    ln -s "$JAVA_HOME/bin/"* "/usr/bin/" && \
    unzip -jo -d "$JAVA_HOME/jre/lib/security" "jce_policy-${JAVA_VERSION}.zip" && \    
    rm -rf "$JAVA_HOME/jre/bin/jjs" \
           "$JAVA_HOME/jre/bin/keytool" \
           "$JAVA_HOME/jre/bin/orbd" \
           "$JAVA_HOME/jre/bin/pack200" \
           "$JAVA_HOME/jre/bin/rmid" \
           "$JAVA_HOME/jre/bin/rmiregistry" \
           "$JAVA_HOME/jre/bin/servertool" \
           "$JAVA_HOME/jre/bin/tnameserv" \
           "$JAVA_HOME/jre/bin/unpack200" \
           "$JAVA_HOME/jre/lib/ext/nashorn.jar" \
           "$JAVA_HOME/jre/lib/jfr.jar" \
           "$JAVA_HOME/jre/lib/jfr" \
           "$JAVA_HOME/jre/lib/oblique-fonts" \           
           "$JAVA_HOME/README.html" \
           "$JAVA_HOME/THIRDPARTYLICENSEREADME-JAVAFX.txt" \
           "$JAVA_HOME/THIRDPARTYLICENSEREADME.txt" \            
           "$JAVA_HOME/jre/README" \
           "$JAVA_HOME/jre/THIRDPARTYLICENSEREADME-JAVAFX.txt" \
           "$JAVA_HOME/jre/THIRDPARTYLICENSEREADME.txt" \
           "$JAVA_HOME/jre/Welcome.html" \
           "$JAVA_HOME/jre/lib/security/README.txt" && \           
    apt-get -y autoremove wget unzip && \
    apt-get -y clean && \
    rm -rf "/tmp/"* \
           "/var/cache/apt" \
           "/usr/share/man" \
           "/usr/share/doc" \
           "/usr/share/doc-base" \
           "/usr/share/info/*"