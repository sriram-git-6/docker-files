# FROM almalinux:8
# RUN cd /tmp
# RUN echo "hello-docker" > hello.txt

# after creating the container from the above docker file the hello.txt will be created in the root directory only.
# To create the file in /tmp directory we need to use WORKDIR instruction.

FROM almalinux:8
WORKDIR /tmp
RUN echo "hello-docker" > hello.txt

# docker run -it workdir:v2 bash ---> directly u will be logged into the /tmp directory.  