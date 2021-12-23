FROM debian

ADD . /tmp

WORKDIR /tmp

RUN dpkg-deb --build debian

RUN apt update; dpkg -i debian.deb; apt-get -f install -y
