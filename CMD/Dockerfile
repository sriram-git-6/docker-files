FROM almalinux:8
# almalinux is same as centos
RUN yum install epel-release -y
# RUN instruction is used to install packages and run commands and run instruction is run at image creation 
RUN yum install nginx -y
RUN echo "Hello, welcome to dockerfile a way of creating own images" > /usr/share/nginx/hello.html
CMD [ "nginx", "-g", "daemon off;" ]
# CMD keeps your container running ..and CMD instruction runs at the time of container creation
