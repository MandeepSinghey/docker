# Docker file for a slim Ubuntu-based Python3 image

FROM ubuntu:latest

RUN apt-get update 
RUN apt-get upgrade -y

RUN apt-get install g++ valgrind -y

RUN apt-get install -y python3-pip python3-dev

RUN cd /usr/local/bin
################################
# Since we created the python to python3
# lik first time, dont need to run  again
# during upgrades
###############################
#RUN ln -s /usr/bin/python3 /usr/local/bin/python
RUN pip3 install --upgrade pip
RUN pip install pandas

