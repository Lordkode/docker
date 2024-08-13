# base image
FROM node:22-alpine as build-stage

# set working directory
WORKDIR /app

# install and cache app dependencies
COPY package*.json .
RUN npm install

COPY . .

EXPOSE 3000

CMD npm run dev