# Start from debian stretch-slim
FROM debian:stretch-slim

# Setup JAVA_HOME
ENV JAVA_HOME="/usr/lib/jvm/default-jvm"

# Install Oracle JDK (Java SE Development Kit) 10.0.1
RUN JAVA_VERSION=10 && \
    JAVA_UPDATE=0.1 && \
    JAVA_BUILD=10 && \
    JAVA_PATH=fb4372174a714e6b8c52526dc134031e && \
    JAVA_SHA256_SUM=ae8ed645e6af38432a56a847597ac61d4283b7536688dbab44ab536199d1e5a4 && \
    apt-get update && \
    apt-get -y install wget && \
    cd "/tmp" && \
    wget --header "Cookie: oraclelicense=accept-securebackup-cookie;" "http://download.oracle.com/otn-pub/java/jdk/${JAVA_VERSION}.${JAVA_UPDATE}+${JAVA_BUILD}/${JAVA_PATH}/jdk-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" && \
    echo "${JAVA_SHA256_SUM}" "jdk-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" | sha256sum -c - && \
    tar -xzf "jdk-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" && \
    mkdir -p "/usr/lib/jvm" && \
    mv "/tmp/jdk-${JAVA_VERSION}.${JAVA_UPDATE}" "/usr/lib/jvm/java-${JAVA_VERSION}-oracle" && \
    ln -s "java-${JAVA_VERSION}-oracle" "$JAVA_HOME" && \
    ln -s "$JAVA_HOME/bin/"* "/usr/bin/" && \
    rm -rf "$JAVA_HOME/README.html" \
           "$JAVA_HOME/bin/javaws" \
           "$JAVA_HOME/bin/jjs" \
           "$JAVA_HOME/bin/keytool" \
           "$JAVA_HOME/bin/orbd" \
           "$JAVA_HOME/bin/pack200" \
           "$JAVA_HOME/bin/policytool" \
           "$JAVA_HOME/bin/rmid" \
           "$JAVA_HOME/bin/rmiregistry" \
           "$JAVA_HOME/bin/servertool" \
           "$JAVA_HOME/bin/tnameserv" \
           "$JAVA_HOME/bin/unpack200" \    
           "$JAVA_HOME/conf/security/javaws.policy" \    
           "$JAVA_HOME/conf/security/policy/README.txt" \ 
           "$JAVA_HOME/lib/desktop" \
           "$JAVA_HOME/lib/"deploy* \
           "$JAVA_HOME/lib/"*javafx* \
           "$JAVA_HOME/lib/"*jfx* \
           "$JAVA_HOME/lib/jfr" \
           "$JAVA_HOME/lib/missioncontrol" \
           "$JAVA_HOME/lib/oblique-fonts" \   
           "$JAVA_HOME/lib/libdecora_sse.so" \
           "$JAVA_HOME/lib/"libprism_*.so \
           "$JAVA_HOME/lib/libfxplugins.so" \
           "$JAVA_HOME/lib/libglass.so" \
           "$JAVA_HOME/lib/libgstreamer-lite.so" \
           "$JAVA_HOME/lib/"libjavafx*.so \
           "$JAVA_HOME/lib/"libjfx*.so \
           "$JAVA_HOME/lib/plugin-legacy.jar" \
           "$JAVA_HOME/lib/plugin.jar" \
           "$JAVA_HOME/lib/src.zip" && \
    apt-get -y autoremove wget && \
    apt-get -y clean && \
    rm -rf "/tmp/"* \
           "/var/cache/apt" \
           "/usr/share/man" \
           "/usr/share/doc" \
           "/usr/share/doc-base" \
           "/usr/share/info/*"