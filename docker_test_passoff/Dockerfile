   # Use an official Python runtime as a parent image
   FROM ubuntu:latest

   RUN apt-get update
   RUN DEBIAN_FRONTEND="noninteractive" apt-get -y install tzdata 
   RUN apt-get -y install apache2 libapache2-mod-php php

   COPY ./charity/ /var/www/html

   EXPOSE 80

   CMD ["/usr/sbin/apache2ctl", "-DFOREGROUND"]

