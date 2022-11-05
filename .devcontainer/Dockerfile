FROM ubuntu:20.04

RUN sed -i 's@archive.ubuntu.com@ftp.jaist.ac.jp/pub/Linux@g' /etc/apt/sources.list \
&& apt update \
&& apt install -y --no-install-recommends apt-utils software-properties-common \
&& add-apt-repository ppa:apt-fast/stable -y\
&& apt install -y --no-install-recommends apt-fast \
&& apt-fast install -y texlive-full latexmk locales\ 
&& locale-gen en_US.UTF-8 && update-locale LANG=en_US.UTF-8

