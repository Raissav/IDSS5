FROM debian
LABEL maintainer="@raissav"
ENV DEBIAN_FRONTEND noninteractive
RUN apt install php8.1 -y
RUN apt-get update && apt-get install -y nginx
RUN usermod -u 1000 www-data

WORKDIR /var/www/html
COPY app/* ./

EXPOSE 80

CMD ["nginx"]
