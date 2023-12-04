FROM almalinux:8
# almalinux is same as centos
RUN yum install epel-release -y
# RUN instruction is used to install packages and run commands and run instruction is run at image creation 
RUN yum install nginx -y
RUN echo "Hello, welcome to dockerfile a way of creating own images" > /usr/share/nginx/html/hello.html
CMD [ "nginx", "-g", "daemon off;" ]
# CMD keeps your container running ..and CMD instruction runs at the time of container creation

# docker run -p 8081:80 cmd:v1 ping google.com --> if u run this command while creating the container 
# it will not run the nginx container that CMD instruction will be overriden with google.com and it will ping
# to google.com.