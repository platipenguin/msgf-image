# Base container
FROM bioconductor/devel_base2

# Maintainer
MAINTAINER Elliot Lee, emlee@fredhutch.org

# Main Directory
WORKDIR /root

# Install Java
RUN apt-get update
RUN apt-get -q -y install default-jdk unzip python2.7 python2.7-dev g++ build-essential libxml2-dev libcurl4-openssl-dev apt-utils libnetcdf-dev
RUN apt-get clean
ENV JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64

# Add MSGF plus
ADD MSGFPlus.jar /root/