FROM ubuntu:bionic
CMD /bin/bash
RUN apt-get update && \
    apt-get --yes upgrade && \
    apt-get --yes dist-upgrade && \
    apt-get --yes install nodejs npm && \
    npm install -g lighthouse && \
    apt-get --yes install chromium-browser
