ARG version
FROM almalinux:${version}
# FROM almalinux:${version:-9} ---> when user forgets to give the version while building the image, we should declare the 
# value like this  
# ARG variable which is defined before FROM instruction will not work after the FROM instruction is executed.

RUN echo "version passed by user is: ${version}"

# docker image build -t arg:v1 --build-arg version=9 .

# after building the image with the above command, FROM instruction will take version 9 but RUN instruction will prints 
# ${version} only. 


# #ARG version
# #FROM almalinux:${version:-8}
# ARG course
# ARG trainer
# RUN echo "course is: ${course}, trainer is: ${trainer}"


# docker image build -t arg:v1 --build-arg course=devops --build-arg trainer=sriram .

# now the variables which are defined with ARG instruction will be displayed because they are declared after the FROM instruction.

# Both ARG and ENV are used for defining variables. But values defined with ARG with not work after your image is built.

# Values defined with ENV are used till your container is created.

# #ARG version
# #FROM almalinux:${version:-8}
# ARG course
# ARG trainer
# ENV COURSE=${course}
# ENV TRAINER=${trainer}
# RUN echo "course is: ${course}, trainer is: ${trainer}"

# If we want to use the ARG variables while creating containers also then create ENV variable and pass the ARG value to the ENV varaible.


