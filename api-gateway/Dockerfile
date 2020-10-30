FROM node: latest

LABEL maintainer="Margret Sol"

COPY . /app
WORKDIR /app

RUN npm install

ENTRYPOINT ["npm", "run", "build"]