#Here selecting the base image for my image
FROM ubuntu 

#Defining working directory in docker container
WORKDIR /app

#Copying script.sh file to docker container
COPY script.sh .

#Giving executable permissions to script.sh file 
RUN chmod +x script.sh

#This is the default command for running the container
CMD ["./script.sh"]