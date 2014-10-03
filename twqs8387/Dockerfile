FROM ubuntu:12.04

RUN \
  apt-get update &&\
  apt-get install -y x11vnc xvfb x11-server-utils firefox &&\
  echo "echo 'Executing xhost +'" >> ~/.bashrc
  echo "xhost +" >> ~/.bashrc

CMD x11vnc -forever -nopw -create

EXPOSE 5900

