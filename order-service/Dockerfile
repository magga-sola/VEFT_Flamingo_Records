FROM node:latest
LABEL maintainer="evan19, margreta19"

ENV ASPNETCORE_URLS=http://+:80

COPY . /app
WORKDIR /app

RUN npm install

ENTRYPOINT [ "npm", "run", "build" ]