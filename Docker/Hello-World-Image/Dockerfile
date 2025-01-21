#Utilizing "ultramcu/ubuntu4bbb" as a base image for build
FROM ultramcu/ubuntu4bbb

#Defining default work directory for image container
WORKDIR /app

#Copying test.cpp in this working directory of docker container
COPY test.cpp .

#Updating the ubuntu terminal packages
RUN sudo apt update 

#Installing g++ in your docker build with "-y" which says yes to any prompts
RUN sudo apt install -y g++

#Running the test.cpp program and storing result in "binaary"
RUN g++ test.cpp -o binary

#Running the container created with image by following command
CMD ["./binary"]


