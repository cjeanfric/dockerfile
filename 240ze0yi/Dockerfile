FROM hopsoft/ruby-mri:2.1.2
RUN \
  apt-get update                                &&\
  apt-get install -y libqt4-dev                 &&\
  apt-get clean                                 &&\
  echo "gem: --no-document" > ~/.gemrc          &&\
  rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

