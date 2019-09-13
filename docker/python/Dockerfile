FROM python:3.6

MAINTAINER Oleg Balditsyn <gluck33@gmail.com>

ENV PROJECT_DIR /srv/www/one_c_adm
ENV SRC_DIR ./one_c_adm

COPY $SRC_DIR $PROJECT_DIR
WORKDIR $PROJECT_DIR
ADD requirements.txt $PROJECT_DIR
RUN apt-get update && apt-get install -y nano
RUN pip install -r requirements.txt
