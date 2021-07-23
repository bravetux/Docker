FROM ubuntu:latest

LABEL maintainer="B.Vignesh Kumar <vigneshkumarb@bravetux.com"

#RUN apt-get update && apt-get install -y locales && rm -rf /var/lib/apt/lists/* \
#    && localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8

RUN apt-get update && \
    apt-get install -y sudo curl git-core gnupg wget zsh bash vim locales nodejs zsh
    npm fonts-powerline && \
    locale-gen en_US.UTF-8 &&
    #adduser --quiet --disabled-password
    #--shell /bin/zsh --home /home/devuser
    #3--gecos "User" devuser && \
    #echo "devuser:<a href="mailto://p@ssword1">p@ssword1</a>" |
    #chpasswd &&  usermod -aG sudo devuser

RUN apt-get install -y build-essential iputils-ping

ENV LANG en_US.utf8

#ADD scripts/installthemes.sh /home/devuser/installthemes.sh
#USER devuser
ENV TERM xterm
ENV ZSH_THEME agnoster
CMD ["/bin/sh"]

