FROM debian:buster
CMD /bin/bash
RUN apt-get update
RUN apt-get --yes upgrade && apt-get --yes dist-upgrade
RUN apt-get --yes install ant proguard openjdk-11-jdk wget unzip apt-utils
ADD https://github.com/pmd/pmd/releases/download/pmd_releases%2F6.13.0/pmd-bin-6.13.0.zip
RUN unzip pmd-bin-6.13.0.zip
