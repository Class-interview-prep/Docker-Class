FROM ubuntu:latest
LABEL maintainer="ikambarov@yahoo.com"
RUN apt-get update -y && apt-get upgrade -y && apt-get install apache2 -y
RUN ln -sf /dev/stdout /var/log/apache2/access.log && ln -sf /dev/stderr /var/log/apache2/error.log
ENV TEST Ubuntu
EXPOSE 80
CMD ["/usr/sbin/apache2ctl",  "-D",  "FOREGROUND"]
