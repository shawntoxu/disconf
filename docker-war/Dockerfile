FROM abc:5000/u14-jdk8-nginx1.8.1:1.0

ADD ./default  /etc/nginx/sites-available/default
COPY ./apache-tomcat-7.0.68 /root/app/tomcat 
ADD ./start.sh /root/start.sh
ADD ./web-app /usr/share/nginx/html
EXPOSE 8080 80 22 

CMD ["/bin/sh","-c","/root/start.sh"]

