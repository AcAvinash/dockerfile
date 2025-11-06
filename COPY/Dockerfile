
FROM almalinux:8

RUN dnf install nginx -y

RUN rm -rf /usr/share/nginx/html/index.html

COPY index.html /usr/share/nginx/html/index.html

COPY qi /usr/share/nginx/html/index.html