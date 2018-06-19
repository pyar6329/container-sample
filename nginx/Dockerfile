FROM nginx:1.15.0

COPY config /tmp/config

RUN set -x \
  && cp -rf /tmp/config/nginx.conf /etc/nginx/nginx.conf \
  && cp -rf /tmp/config/default.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
