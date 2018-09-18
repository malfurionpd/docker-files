# from sbt
FROM hseeberger/scala-sbt:8u171_2.12.6_1.1.6
MAINTAINER adeng <343753091@qq.com>

# add repositories
ADD repositories /root/.sbt

# mkdir before sbt run
RUN mkdir /root/.ivy2

# docker client
RUN wget -P /tmp/ https://download.docker.com/linux/static/stable/x86_64/docker-18.06.1-ce.tgz && \
    tar -xvf /tmp/docker-18.06.1-ce.tgz --directory /tmp/ && \
    mv /tmp/docker/docker /usr/local/bin
