FROM almalinux:8
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# ONBUILD insruction will not execute at the time of image creation.
ONBUILD ADD index.html /usr/share/nginx/html/index.html
CMD [ "nginx", "-g", "daemon off;" ] 

# Image will be created from the above docker file without error. Because onbuild instruction will not be executed at the time 

# of image creation.

# Now create one docker file and use this image as the base image to create an image.

# FROM onbuild:v1(image created using the above docker file)

# create an image from the above docker file. Now you will get an error because index.html file is not present.

# create index.html file and create image from the above docker file now you wont get any error.

# now create container from the image (docker run -d -p 80:80 test-onbuild:v1)


