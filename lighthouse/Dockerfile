FROM ubuntu:bionic
CMD /bin/bash
RUN apt-get update
RUN apt-get --yes install dpkg
RUN apt-get --yes install nodejs npm wget dpkg && \
    npm install -g lighthouse && \
    wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb && \
    dpkg -i ./google-chrome-stable_current_amd64.deb && \
    apt-get --yes install -f
