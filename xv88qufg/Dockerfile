FROM dockerfile/nodejs

RUN \
  apt-get update                                &&\
  apt-get install -y ruby                       &&\
  rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* &&\
  echo "gem: --no-document" > ~/.gemrc          &&\
  gem install bundler                           &&\
  npm install -g grunt-cli bower   
