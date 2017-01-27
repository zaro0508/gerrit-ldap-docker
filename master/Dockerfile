FROM gerritforge/gerrit-ubuntu15.04:2.13.5

USER root

RUN apt-get install -y net-tools netcat inetutils-ping openjdk-8-jdk && \
    update-java-alternatives -v -s java-1.8.0-openjdk-amd64

ADD start.sh /bin/

ADD wait-for-it.sh /bin/

CMD /bin/start.sh
