FROM dockerfile/nodejs

RUN \
  apt-get update                                                   &&\
  apt-get install -y ruby                                          &&\
  echo "gem: --no-document" > /root/.gemrc                         &&\
  gem install bundler                                              &&\
  npm install -g grunt-cli bower                                   &&\
  rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
