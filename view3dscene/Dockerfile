FROM ubuntu:12.04
MAINTAINER UberConverter <admin@uberconverter.com>

RUN apt-get update
RUN apt-get install -y libgtkglext1
RUN apt-get install -y wget

# Install vnc, xvfb in order to create a 'fake' display
RUN apt-get install -y x11vnc xvfb
# RUN mkdir /.vnc
# Setup a password
# RUN x11vnc -storepasswd 1234 ~/.vnc/passwd

RUN wget http://downloads.sourceforge.net/castle-engine/view3dscene-3.13.0-linux-x86_64.tar.gz
RUN tar xvfz view3dscene-3.13.0-linux-x86_64.tar.gz

# ["x11vnc", "-forever", "-usepw", "-create"]
