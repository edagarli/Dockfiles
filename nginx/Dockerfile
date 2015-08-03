FROM ubuntu:14.04
MAINTAINER edagarli "edagarli@lydiabox.com"
ENV REFRESHED_AT 2014-06-01
RUN apt-get update
RUN apt-get -y -q install nginx
RUN apt-get install -y curl git
RUN mkdir -p /var/www/html/
RUN git clone https://justpower:www016211abc@git.oschina.net/justpower/website.git /var/www/html
#RUN mkdir -p /var/www/
#RUN ls /var/www/html/
ADD nginx/global.conf /etc/nginx/conf.d/
ADD nginx/nginx.conf /etc/nginx/nginx.conf
EXPOSE 80

CMD [ "/bin/bash"]
