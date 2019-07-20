#install os
FROM ubuntu

RUN apt-get update \ 
   && apt-get install -y apache2

#copy hi.html file in apache2(web server)
COPY hi.html /var/www/html/

#virtual directory which need to expose
WORKDIR /var/www/html

#start apache2 services 
CMD ["apachectl", "-D", "FOREGROUND"]

#expose to port
EXPOSE 80
