# FROM almalinux:8
# RUN echo "hello-docker" > /tmp/hello.txt

# After creating the container from the above docker file the container will be running with root user. 



FROM almalinux:8
RUN useradd sriram
USER sriram
RUN echo "hello-docker" > /tmp/hello.txt

# After creating the container from the above docker file the container will be running with sriram user. 

