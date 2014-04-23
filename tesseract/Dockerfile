FROM ubuntu:12.04
MAINTAINER UberConverter <admin@uberconverter.com>

# non interactive apt
ENV DEBIAN_FRONTEND noninteractive

ENV TESSERACT_VERSION 3.02.02
ENV TESSDATA_VERSION 3.02
ENV TESSDATA_OSD 3.01.osd

# Install required packages
RUN apt-get -q -y update \
    && apt-get -q -y -f install autoconf automake libtool libpng12-dev libjpeg62-dev \
    libgif-dev zlib1g-dev

RUN apt-get -q -y install libtiff4-dev libleptonica-dev libboost-thread-dev
     
# Download files
RUN mkdir /opt/tesseract && cd /opt/tesseract \
    && curl https://tesseract-ocr.googlecode.com/files/tesseract-ocr-$TESSERACT_VERSION.tar.gz | tar -xz \
    && curl https://tesseract-ocr.googlecode.com/files/tesseract-ocr-$TESSDATA_VERSION.eng.tar.gz | tar -xz \
    && curl https://tesseract-ocr.googlecode.com/files/tesseract-ocr-$TESSDATA_OSD.tar.gz | tar -xz

# Compile Tesseract
RUN cd /opt/tesseract/tesseract-ocr \
    && ./autogen.sh && ./configure && make && make install && ldconfig




CMD ["/usr/local/bin/tesseract", "--help"]
