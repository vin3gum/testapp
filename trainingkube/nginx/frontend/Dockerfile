FROM ubuntu:18.04
MAINTAINER vin3_gum@yahoo.com
RUN apt-get -y update
RUN apt-get -y install tzdata
ENV TZ = Asia/Kolkata
ADD config /opt
RUN apt-get -y install `cat /opt/nginxphp`
RUN apt-get -y install `cat /opt/phpgenericmod`
RUN apt-get -y install `cat /opt/phpprojectmod`
ADD code /var/www/html
ENV BACKENDLB=test
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]