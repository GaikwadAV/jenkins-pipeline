FROM ubuntu:latest

RUN yum -y update && yum -y install nginx

COPY index.html /var/www/html/index.nginx-debian.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
