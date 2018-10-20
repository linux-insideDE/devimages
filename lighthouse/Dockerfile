FROM ubuntu:bionic
CMD /bin/bash
RUN apt-get update && \
    apt-get --yes upgrade && \
    apt-get --yes dist-upgrade && \
    apt-get --yes install nodejs npm wget dpkg && \
    npm install -g lighthouse && \
    wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb && \
    apt install ./google-chrome-stable_current_amd64.deb
