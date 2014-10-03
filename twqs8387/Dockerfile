FROM ubuntu:12.04

RUN \
  apt-get update &&\
  apt-get install -y x11vnc xvfb firefox

RUN \
  apt-get install xhost &&\
  echo "xhost +" >> /root/.bashrc

CMD x11vnc -forever -nopw -create

VOLUMES ["/tmp/.X11-unix"]

EXPOSE 5900
