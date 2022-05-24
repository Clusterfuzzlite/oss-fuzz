FROM gcr.io/oss-fuzz-base/base-builder-python:v1
RUN apt-get update && apt-get install -y make autoconf automake libtool

RUN git clone https://github.com/syedafazilathjahaa/Dvpwa.git

COPY . $SRC/Dvpwa
WORKDIR Dvpwa

RUN pip3 install --upgrade pip
RUN pip3 install lz4 --force
RUN pip3 install idna --force
RUN pip3 install atheris --force

COPY *.py $SRC/
