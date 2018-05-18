FROM ubuntu:16.04
MAINTAINER DrTrigon <dr.trigon@surfeu.ch>

# LABEL author.user1="DrTrigon <dr.trigon@surfeu.ch>"

## Environment Variables
#ENV ARDUINO_VERSION 1.8.2
##ENV BOARD "arduino:avr:nano:cpu=atmega328"

# Initial update
RUN apt-get -y update

# Basic packages
RUN apt-get install -y \
  kubuntu-desktop \
  wget

## xz (for tar)
#RUN apt-get install -y xz-utils
#
## binutils (for readelf)
#RUN apt-get install -y binutils

# tree
RUN apt-get install -y tree

# Install Arduino IDE
RUN wget https://github.com/Distroshare/distroshare-ubuntu-imager/archive/v1.0.15.tar.gz
RUN tar xzf v1.0.15.tar.gz

# debug
RUN tree

RUN cd ~/distroshare-ubuntu-imager-1.0; ./distroshare-ubuntu-imager.sh

# debug
RUN ls -la ~/distroshare-ubuntu-imager-1.0
