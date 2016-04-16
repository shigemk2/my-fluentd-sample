FROM alpine:latest
RUN apk add --update nginx && rm -rf /var/cache/apk/* && \
 mkdir -p /tmp/nginx/client-body

COPY conf/nginx.conf /etc/nginx/nginx.conf

CMD ["nginx", "-g", "daemon off;"]