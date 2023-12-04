FROM almalinux:8
# almalinux is same as centos
RUN yum install epel-release -y
# RUN instruction is used to install packages and run commands and run instruction is run at image creation 
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
RUN echo "Hello, welcome to dockerfile a way of creating own images" > /usr/share/nginx/html/index.html
ENTRYPOINT  [ "nginx", "-g", "daemon off;" ]
# Entrypoint keeps your container running ..and CMD instruction runs at the time of container creation.
# Entrypoint cannot be overridden.
# docker run -p 8081:80 entry:v1 ping google.com --> if u run this command while creating the container 
# entrypoint instruction will not be overriden with ping google.com.

