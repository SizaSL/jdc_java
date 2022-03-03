FROM ubuntu:18.04

RUN apt-get update
RUN rm /bin/sh && ln -s /bin/bash /bin/sh
RUN apt-get -qq -y install curl wget unzip zip

RUN curl -s "https://get.sdkman.io" | bash
RUN source "$HOME/.sdkman/bin/sdkman-init.sh" && \
   sdk install java 17.0.2-ms && \
   sdkman_auto_answer=false sdk install java 11.0.14-ms