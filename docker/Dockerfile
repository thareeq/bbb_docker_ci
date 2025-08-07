FROM debian:bullseye

RUN dpkg --add-architecture armhf && \
    apt-get update && \
    apt-get install -y \
    gcc-arm-linux-gnueabihf \
    g++-arm-linux-gnueabihf \
    libc6-dev-armhf-cross \
    g++-arm-linux-gnueabihf \
    gcc-arm-linux-gnueabihf \
    cmake \
    make \
    git \
    cppcheck \
    valgrind

WORKDIR /app
