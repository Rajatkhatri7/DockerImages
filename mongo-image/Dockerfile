# step1

#base image to interact with kernal I/o etc

#can use any os other than alpine
FROM alpine 



# step2 install a software
RUN echo 'http://dl-cdn.alpinelinux.org/alpine/v3.6/main' >> /etc/apk/repositories


RUN echo 'http://dl-cdn.alpinelinux.org/alpine/v3.6/community' >> /etc/apk/repositories


RUN apk update 
RUN apk add mongodb=3.4.4-r0

#step 2.5 configure software
VOLUME [ "/data/db" ]

WORKDIR /data

EXPOSE 27017



# step3 set default commands
CMD [ "mongod" ]




