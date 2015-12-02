FROM centos:latest
MAINTAINER Chao<chaopeng@chaopeng.me>

RUN yum install -y unzip && \
    yum clean all

RUN curl -L -s get.jenv.io | bash && \
    source "/root/.jenv/bin/jenv-init.sh" && \
    jenv repo update && \
    jenv config auto true && \
    jenv install java 1.8.0_60 && \
    jenv clean && \
    rm -rf /root/.jenv/candidates/java/current/javafx-src.zip /root/.jenv/candidates/java/current/src.zip /root/.jenv/candidates/java/current/man /root/.jenv/candidates/java/current/jre
    
env PATH /root/.jenv/candidates/java/current/bin:$PATH
