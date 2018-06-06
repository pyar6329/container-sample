FROM ubuntu:16.04

COPY entrypoint.sh /usr/bin/entrypoint.sh

RUN set -x \
      && apt-get update -y \
      && apt-get install -y nginx \
      && chmod +x /usr/bin/entrypoint.sh

CMD ["entrypoint.sh"]
