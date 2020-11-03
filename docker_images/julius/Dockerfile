FROM ubuntu:latest

RUN apt update -y
RUN apt install -y build-essential zlib1g-dev libsdl2-dev libasound2-dev curl
RUN curl -L https://github.com/julius-speech/julius/archive/v4.6.tar.gz -o julius.tar.gz
RUN tar zxvf julius.tar.gz && cd julius-4.6 && ./configure --with-mictype=pulseaudio && make && make install
RUN sh
