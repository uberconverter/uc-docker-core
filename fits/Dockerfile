# FITS
#
# VERSION 0.8.0

FROM jdk7
MAINTAINER UberConverter <admin@uberconverter.com>

RUN apt-get install -y unzip file
RUN wget -q -O /opt/fits.zip http://projects.iq.harvard.edu/files/fits/files/fits-0.8.0.zip
RUN cd /opt/ && unzip fits.zip && ln -s fits-0.8.0 fits && chmod a+x fits/fits.sh

