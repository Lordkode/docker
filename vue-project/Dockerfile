# base image
FROM node:22-alpine as build-stage

# set working directory
WORKDIR /app

# install and cache app dependencies
COPY package*.json .
RUN npm install

COPY . .

RUN npm run build


FROM nginx:stable-alpine as production-stage
COPY --from=build-stage /app/dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]