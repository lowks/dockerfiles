FROM ubuntu
MAINTAINER Low Kian Seong <kianseong@gmail.com>

RUN apt-get update
RUN apt-get install -y curl build-essential
RUN mkdir /home/lowks
RUN adduser --disabled-password --gecos '' lowks
RUN adduser lowks sudo
echo '%sudo ALL=(ALL) NOPASSWD:ALL' >> /etc/sudoers
RUN curl -s https://static.rust-lang.org/rustup.sh | sh
