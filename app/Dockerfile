# syntax=docker/dockerfile:1

FROM mhart/alpine-node:latest

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install

COPY . .

EXPOSE 80
CMD [ "node", "server.js" ]
