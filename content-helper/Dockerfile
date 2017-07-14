FROM node:6-alpine

RUN mkdir /npm

COPY ./package.json /npm/package.json

WORKDIR /npm

RUN npm i

VOLUME /npm/node_modules
