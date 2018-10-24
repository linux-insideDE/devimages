FROM ubuntu:bionic
CMD /bin/bash
RUN apt-get update
RUN apt-get --yes upgrade && apt-get --yes dist-upgrade
RUN apt-get --yes install nodejs npm wget software-properties-common apt-utils && \
    npm install -g lighthouse
RUN wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -
RUN echo 'deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main' > /etc/apt/sources.list.d/google-chrome.list
RUN apt-get update && apt-get --yes install google-chrome-stable
