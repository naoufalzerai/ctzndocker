FROM nginx:stable-alpine
RUN apk add --no-cache certbot

COPY proxy/renew /etc/periodic/daily/renew
RUN chmod +x /etc/periodic/daily/renew

RUN mkdir /var/lib/certbot

COPY proxy/entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

COPY proxy/nginx.conf /etc/nginx/nginx.conf

ENTRYPOINT [ "../entrypoint.sh" ]