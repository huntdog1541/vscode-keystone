FROM ubuntu 

RUN apt-get update && apt-get upgrade -y \
    && apt-get install -y build-essential git cmake python \
    && git clone https://github.com/keystone-engine/keystone.git \
    && cd keystone && mkdir build && cd build && ../make-share.sh \
    && make install && kstool x32 "add eax, ebx"
