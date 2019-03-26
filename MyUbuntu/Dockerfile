FROM ubuntu

# install packages
RUN apt-get update &&\
    apt-get -y install python-minimal mc wget vim bash-completion

#make tab-completion working in console
RUN apt-get -y install bash-completion

RUN echo "# enable bash completion in interactive shells" >> /etc/bash.bashrc
RUN echo "if ! shopt -oq posix; then" >> /etc/bash.bashrc
RUN echo "if [ -f /usr/share/bash-completion/bash_completion ]; then" >> /etc/bash.bashrc
RUN echo ". /usr/share/bash-completion/bash_completion" >> /etc/bash.bashrc
RUN echo "elif [ -f /etc/bash_completion ]; then" >> /etc/bash.bashrc
RUN echo ". /etc/bash_completion" >> /etc/bash.bashrc
RUN echo "fi" >> /etc/bash.bashrc
RUN echo "fi" >> /etc/bash.bashrc

#enjoy it ;)
