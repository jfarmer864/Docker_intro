FROM ubuntu:16.04

RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install python-software-properties -y
RUN apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_12.x | bash
RUN apt-get install nodejs -y
ADD app /home/ubuntu/app

WORKDIR /home/ubuntu/app
RUN npm install
EXPOSE 3000

CMD ["node", "app.js"]

