FROM node:latest

RUN apt-get update && apt-get upgrade -y
RUN apt-get install wget git

RUN git clone https://github.com/kcm0147/SmartFactory.git
WORKDIR /SmartFactory/Client

RUN npm install

ENTRYPOINT [ "npm" ]
CMD ["start"]