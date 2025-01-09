FROM ubuntu:24.04

RUN apt update && apt install apt-utils && echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections && apt install -y cmatrix && rm -rf /var/lib/apt

ENTRYPOINT [ "/usr/bin/cmatrix" ]