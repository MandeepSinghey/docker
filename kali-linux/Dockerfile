# Kali Linux Top10
# Docker image with kali-linux-top10 and a handful of other useful tools
# More info: https://medium.com/@infosec_stuff/kali-linux-in-a-docker-container-5a06311624eb

FROM kalilinux/kali-linux-docker

ENV DEBIAN_FRONTEND noninteractive
# do APT update
RUN apt-get -y update && apt-get -y dist-upgrade && apt-get -y autoremove && apt-get clean
# install Kali Linux "Top 10" metapackage and a couple "nice to have" tools
RUN apt-get -y install kali-linux-top10 exploitdb man-db dirb nikto wpscan uniscan
RUN apt-get -y install ncrack

WORKDIR /root
ENTRYPOINT ["/bin/bash"]

    