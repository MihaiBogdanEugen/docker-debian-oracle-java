# Start from debian stretch-slim
FROM debian:stretch-slim

# Setup JAVA_HOME
ENV JAVA_HOME="/usr/lib/jvm/default-jvm"

# Install Oracle Server JRE (Java SE Runtime Environment) 10.0.2
RUN JAVA_VERSION=10 && \
    JAVA_UPDATE=0.2 && \
    JAVA_BUILD=13 && \
    JAVA_PATH=19aef61b38124481863b1413dce1855f && \
    JAVA_SHA256_SUM=4ca492e0dd46c51bb3263d7347f6ede04fceb07fde3f01fed2c0336b18596c41 && \
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
           "$JAVA_HOME/conf/security/policy/README.txt" \            
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