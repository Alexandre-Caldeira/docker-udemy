# create your custom drupal image here, based of official drupal
FROM drupal:8

RUN apt-get update && apt-get install -y git \
    && rm -rf /var/lib/apt/lists/* \
    && cd /var/www/html/themes \
    && git clone --branch 8.x-3.x --single-branch --depth 1 https://git.drupal.org/project/bootstrap.git

WORKDIR /var/www/html

