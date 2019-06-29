FROM ubuntu:16.04

WORKDIR /app
COPY . .
RUN apt-get update && apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
RUN npm install -g serve
RUN npm install --save-dev webpack
RUN npm audit fix
RUN chmod a+rx /app
CMD ["npm", "start"]
