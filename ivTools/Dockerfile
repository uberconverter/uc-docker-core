FROM ubuntu:12.04
MAINTAINER UberConverter <admin@uberconverter.com>

RUN apt-get update 

RUN apt-get install -y software-properties-common
RUN apt-get install -y python-software-properties
RUN add-apt-repository -y ppa:ubuntu-wine/ppa

RUN apt-get update 

RUN apt-get -y install wine

ADD win-exes /opt/ivTools

