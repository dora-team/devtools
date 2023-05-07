FROM us-central1-docker.pkg.dev/cloud-workstations-images/predefined/code-oss:latest

RUN wget https://github.com/gohugoio/hugo/releases/download/v0.111.3/hugo_extended_0.111.3_Linux-64bit.tar.gz
RUN tar -xf ./hugo_extended_0.111.3_Linux-64bit.tar.gz
RUN mv hugo /usr/local/bin
RUN rm ./hugo_extended_0.111.3_Linux-64bit.tar.gz