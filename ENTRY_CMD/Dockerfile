FROM almalinux:8
ENTRYPOINT [ "ping", "-c5", "facebook.com" ]

# docker run entry:v2 ---> it will ping for facebook.com for 5 times.
# docker run entry:v2 ping google.com ---> entrypoint will not override with ping google.com
# docker ps -a --no-trunc ---> it shows all the containers(running and exited) and the command that is given 
# to run the container.
# And the command field shows ping -c5 facebook.com google.com ---> means google.com is getting appending to ping command.
# you cant override entrypoint if u try to override it will go and append to the entrypoint command mentioned in docker file.

FROM almalinux:8
ENTRYPOINT [ "ping", "-c5" ]

# docker run entry:v2 google.com  ----> now it will ping google.com means here it is appending to ping command.

# so for best results we combine entrypoint with cmd.

FROM almalinux:8
ENTRYPOINT [ "ping", "-c5" ]
CMD [ "google.com" ]

# docker run entry:v2 yahoo.com ---->now it will override because of cmd