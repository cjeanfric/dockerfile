FROM hopsoft/ruby-mri:2.1.2
RUN \
  apt-get update                                &&\
  apt-get install -y libqt4-dev                 &&\
  apt-get clean                                 &&\
  rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

