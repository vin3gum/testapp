FROM centos:7
MAINTAINER vin3_gum@yahoo.com
RUN yum -y update
RUN yum -y install httpd
ADD code /var/www/html
ENV BACKENDLB=test
EXPOSE 80
CMD ["apachectl", "-D", "FOREGROUND"]