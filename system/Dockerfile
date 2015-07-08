# System Image
#
# - Ubuntu 14.04
# - phpbrew requirements
# - git
# - composer

FROM  ubuntu:14.04

RUN apt-get update \
  && apt-get build-dep -y php5 \
  && apt-get install -y php5 php5-dev php-pear autoconf automake curl build-essential libxslt1-dev re2c libxml2 libxml2-dev php5-cli bison libbz2-dev libreadline-dev \
  && apt-get install -y libfreetype6 libfreetype6-dev libpng12-0 libpng12-dev libjpeg-dev libjpeg8-dev libjpeg8  libgd-dev libgd3 libxpm4 libltdl7 libltdl-dev \
  && apt-get install -y libssl-dev openssl \
  && apt-get install -y gettext libgettextpo-dev libgettextpo0 \
  && apt-get install -y libicu-dev \
  && apt-get install -y libmhash-dev libmhash2 \
  && apt-get install -y libmcrypt-dev libmcrypt4 \
  && apt-get install -y mysql-server mysql-client libmysqlclient-dev libmysqld-dev \
  && apt-get install -y ca-certificates \
  && apt-get install -y libyaml-dev \
  && apt-get install -y libcurl4-gnutls-dev libexpat1-dev libz-dev \
  && apt-get install -y git \
  && curl -sS https://getcomposer.org/installer | php \
  && mv composer.phar /usr/local/bin/composer \
  && apt-get clean -y\
  && apt-get autoclean -y \
  && apt-get autoremove -y

