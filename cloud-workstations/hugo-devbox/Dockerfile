FROM gcr.io/doradotdev/dora-team-base-config:latest

RUN wget https://github.com/gohugoio/hugo/releases/download/v0.118.2/hugo_extended_0.118.2_Linux-64bit.tar.gz
RUN tar -xf ./hugo_extended_0.118.2_Linux-64bit.tar.gz
RUN mv hugo /usr/local/bin
RUN rm ./hugo_extended_0.118.2_Linux-64bit.tar.gz
