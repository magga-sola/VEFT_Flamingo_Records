FROM node:latest
LABEL maintainer="evan19, margreta19"


COPY . /app
WORKDIR /app

RUN npm install

ENTRYPOINT [ "npm", "run", "build" ]