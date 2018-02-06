# Start from debian stretch-slim
FROM debian:stretch-slim

# Setup JAVA_HOME
ENV JAVA_HOME="/usr/lib/jvm/default-jvm"

# Install Oracle Server JRE (Java SE Runtime Environment) 9.0.4
RUN JAVA_VERSION=9 && \
    JAVA_UPDATE=0.4 && \
    JAVA_BUILD=11 && \
    JAVA_PATH=c2514751926b4512b076cc82f959763f && \
    JAVA_SHA256_SUM=d29b6b3008c814abd8ab5e4bde9278d6ee7699898333992ee8d080612b5197ca && \
    apt-get update && \
    apt-get -y install wget && \
    cd "/tmp" && \
    wget --header "Cookie: oraclelicense=accept-securebackup-cookie;" "http://download.oracle.com/otn-pub/java/jdk/${JAVA_VERSION}.${JAVA_UPDATE}+${JAVA_BUILD}/${JAVA_PATH}/serverjre-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" && \
    echo "${JAVA_SHA256_SUM}" "serverjre-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" | sha256sum -c - && \
    tar -xzf "serverjre-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" && \
    mkdir -p "/usr/lib/jvm" && \
    mv "/tmp/jdk-${JAVA_VERSION}.${JAVA_UPDATE}" "/usr/lib/jvm/java-${JAVA_VERSION}-oracle" && \
    ln -s "java-${JAVA_VERSION}-oracle" "$JAVA_HOME" && \
    ln -s "$JAVA_HOME/bin/"* "/usr/bin/" && \
    rm -rf "$JAVA_HOME/README.html" \
           "$JAVA_HOME/bin/keytool" \
           "$JAVA_HOME/bin/rmid" \
           "$JAVA_HOME/bin/rmiregistry" \
           "$JAVA_HOME/lib/"*javafx* \
           "$JAVA_HOME/lib/"*jfx* \
           "$JAVA_HOME/lib/jfr" \
           "$JAVA_HOME/lib/oblique-fonts" && \
    apt-get -y autoremove wget && \
    apt-get -y clean && \
    rm -rf "/tmp/"* \
           "/var/cache/apt" \
           "/usr/share/man" \
           "/usr/share/doc" \
           "/usr/share/doc-base" \
           "/usr/share/info/*"