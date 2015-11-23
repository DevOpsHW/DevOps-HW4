FROM    ubuntu:14.04

# Install Node.js and npm
RUN	apt-get update
RUN	apt-get -y install git
RUN	apt-get -y install nodejs
RUN	apt-get -y install npm
# Bundle app source
COPY ./App /src
# Install app dependencies
RUN cd /src; npm install

EXPOSE  8080
CMD ["nodejs", "/src/main.js", "8080"]
