FROM ubuntu:14.04
MAINTAINER edagarli "edagarli@lydiabox.com"
ENV REFRESHED_AT 2014-06-01
RUN apt-get update
RUN apt-get -y -q install nginx
RUN apt-get install -y curl git
RUN mkdir -p /var/www/html/
RUN git clone https://justpower:www016211abc@git.oschina.net/justpower/website.git /var/www/html
RUN mkdir -p /var/www/dockerfiles/
Run git clone https://github.com/edagarli/Dockfiles /var/www/dockerfiles/
RUN cd /var/www/dockerfiles/
ADD nginx/nginx/global.conf /etc/nginx/conf.d/
ADD nginx/nginx/nginx.conf /etc/nginx/nginx.conf
#RUN curl -fL https://raw.githubusercontent.com/edagarli/Dockfiles/master/nginx/nginx/global.conf -o /etc/nginx/conf.d/global.conf
#RUN curl -fL https://github.com/edagarli/Dockfiles/blob/master/nginx/nginx/nginx.conf -o /etc/nginx/nginx.conf
EXPOSE 80

#CMD [ "/bin/bash"]
