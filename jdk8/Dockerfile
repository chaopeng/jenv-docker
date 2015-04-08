FROM centos:latest
MAINTAINER Chao<chaopeng@chaopeng.me>

RUN yum install -y unzip

RUN curl -L -s get.jenv.io | bash && \
    source "/root/.jenv/bin/jenv-init.sh" && \
    jenv repo update && \
    jenv config auto true && \
    jenv install java 1.8.0_40
    
env PATH /root/.jenv/candidates/java/current/bin:$PATH
