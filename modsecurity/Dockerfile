FROM krish512/modsecurity

#RUN apt update
#RUN apt upgrade -y
#RUN apt install openssl
#RUN openssl req -newkey rsa:4096 -x509 -sha256 -days 365 -nodes -out /etc/nginx/server.crt -keyout /etc/nginx/server.key -subj "/C=US/ST=NY/L=Rochester/O=RIT/OU=CSEC731/CN=www.dockerdemo.com"

COPY server.crt /etc/nginx/server.crt
COPY server.key /etc/nginx/server.key


RUN rm /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/conf.d/


