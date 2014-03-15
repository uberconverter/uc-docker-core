# Blender
#
# VERSION 1.0

FROM ubuntu:12.04
MAINTAINER UberConverter <admin@uberconverter.com>

RUN apt-get update
RUN apt-get install -y software-properties-common
RUN apt-get install -y python-software-properties
RUN add-apt-repository ppa:irie/blender && apt-get update

# For Blender 2.68.x
RUN apt-get install -y blender

# Add scripts for performing conversions
ADD wrl2x3d /opt/wrl2x3d

