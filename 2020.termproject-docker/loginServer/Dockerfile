FROM node:latest

RUN apt-get update && apt-get upgrade -y

RUN git clone https://github.com/kcm0147/SmartFactory.git
RUN pwd
WORKDIR /SmartFactory/loginServer

RUN npm install

CMD ["index.js"]
# ENTRYPOINT [ "./run_endpoint.sh" ]