# Start from debian stretch-slim
FROM debian:stretch-slim

# Setup JAVA_HOME
ENV JAVA_HOME="/usr/lib/jvm/default-jvm"

# Install Oracle JRE (Java SE Runtime Environment) 9.0.1
RUN JAVA_VERSION=9 && \
    JAVA_UPDATE=0.1 && \
    JAVA_BUILD=11 && \
    JAVA_SHA256_SUM=3c64953465e98dbab0e449954a918fada703cd0341aa98cff68854852663ee86 && \
    apt-get update && \
    apt-get -y install wget && \
    cd "/tmp" && \
    wget --header "Cookie: oraclelicense=accept-securebackup-cookie;" "http://download.oracle.com/otn-pub/java/jdk/${JAVA_VERSION}.${JAVA_UPDATE}+${JAVA_BUILD}/jre-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" && \
    echo "${JAVA_SHA256_SUM}" "jre-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" | sha256sum -c - && \
    tar -xzf "jre-${JAVA_VERSION}.${JAVA_UPDATE}_linux-x64_bin.tar.gz" && \
    mkdir -p "/usr/lib/jvm" && \
    mv "/tmp/jre-${JAVA_VERSION}.${JAVA_UPDATE}" "/usr/lib/jvm/java-${JAVA_VERSION}-oracle" && \
    ln -s "java-${JAVA_VERSION}-oracle" "$JAVA_HOME" && \
    ln -s "$JAVA_HOME/bin/"* "/usr/bin/" && \
    rm -rf "$JAVA_HOME/README.html" \
           "$JAVA_HOME/bin/javaws" \
           "$JAVA_HOME/bin/jjs" \
           "$JAVA_HOME/bin/keytool" \
           "$JAVA_HOME/bin/orbd" \
           "$JAVA_HOME/bin/pack200" \
           "$JAVA_HOME/bin/rmid" \
           "$JAVA_HOME/bin/rmiregistry" \
           "$JAVA_HOME/bin/servertool" \
           "$JAVA_HOME/bin/tnameserv" \
           "$JAVA_HOME/bin/unpack200" \    
           "$JAVA_HOME/conf/security/javaws.policy" \    
           "$JAVA_HOME/lib/desktop" \
           "$JAVA_HOME/lib/"deploy* \
           "$JAVA_HOME/lib/"*javafx* \
           "$JAVA_HOME/lib/"*jfx* \
           "$JAVA_HOME/lib/jfr" \
           "$JAVA_HOME/lib/oblique-fonts" \   
           "$JAVA_HOME/lib/libdecora_sse.so" \
           "$JAVA_HOME/lib/"libprism_*.so \
           "$JAVA_HOME/lib/libfxplugins.so" \
           "$JAVA_HOME/lib/libglass.so" \
           "$JAVA_HOME/lib/libgstreamer-lite.so" \
           "$JAVA_HOME/lib/"libjavafx*.so \
           "$JAVA_HOME/lib/"libjfx*.so \
           "$JAVA_HOME/lib/plugin-legacy.jar" \
           "$JAVA_HOME/lib/plugin.jar" && \
    apt-get -y autoremove wget && \
    apt-get -y clean && \
    rm -rf "/tmp/"* \
           "/var/cache/apt" \
           "/usr/share/man" \
           "/usr/share/doc" \
           "/usr/share/doc-base" \
           "/usr/share/info/*"