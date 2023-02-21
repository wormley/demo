FROM debian:stable-slim

COPY requirements.txt /data/requirements.txt

WORKDIR /data

RUN apt update; apt install -y locales-all sshpass;\
    apt install -y python3; \
    apt install -y python3-pip; \
    apt install -y git

RUN python3 -m pip install --upgrade pip; \
    python3 -m pip install -r requirements.txt
