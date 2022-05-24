FROM gcr.io/oss-fuzz-base/base-builder-python:v1
RUN apt-get update && apt-get install -y make autoconf automake libtool

COPY . $SRC/Dvpwa
WORKDIR Dvpwa

RUN git clone --depth=1 https://github.com/syedafazilathjahaa/Dvpwa.git Dvpwa
RUN pip3 install --upgrade pip
RUN pip3 install lz4 --force
RUN pip3 install idna --force
RUN pip3 install atheris --force
