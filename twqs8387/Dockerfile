FROM ubuntu:12.04

RUN \
  apt-get update &&\
  apt-get install -y x11vnc xvfb x11-xserver-utils firefox xterm fvwm &&\
  rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* &&\
  \
  echo "Xvfb :20 -screen 0 1280x1024x24 -cc 4 -nolisten tcp &" >  start.sh &&\
  echo "xterm -e 'xhost +'"                                    >> start.sh &&\
  echo "x11vnc -forever -nopw -display :20"                    >> start.sh

CMD /bin/sh start.sh

EXPOSE 5900
