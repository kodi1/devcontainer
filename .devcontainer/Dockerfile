FROM ubuntu:24.04

ENV TZ=Europe/Sofia

RUN apt-get update &&\
     DEBIAN_FRONTEND=noninteractive apt-get install --install-recommends -y \
     apt-transport-https\
     gpg\
     curl\
     wget\
     sudo\
     ssh\
     git\
     git-lfs\
     unzip\
     gitk\
     flex\
     bison\
     libssl-dev\
     bc\
     libxml-simple-perl\
     rsync\
     dos2unix\
     libxml2-utils\
     libasound2-dev\
     lsb-release\
     software-properties-common\
     gdb\
     build-essential\
     vim\
     tzdata\
     libtool\
     pkg-config\
     bash-completion\
     python3\
     python3-pip\
     python3-setuptools\
     python3-wheel\
     python3-venv\
     clang\
     clangd\
     && ln -fs /usr/bin/python3 /usr/bin/python

RUN useradd -m -r -s /bin/bash appuser &&\
     echo 'appuser ALL=(ALL) NOPASSWD:SETENV: ALL' >> /etc/sudoers &&\
     echo 'StrictHostKeyChecking no' >> /etc/ssh/ssh_config &&\
     echo '. /etc/bash_completion' >> /etc/bash.bashrc
