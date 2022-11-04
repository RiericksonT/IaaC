FROM node:16.13.0

WORKDIR /usr/src/client

COPY *.json ./

RUN npm install @quasar/cli

RUN npm install

COPY . .

EXPOSE 3000