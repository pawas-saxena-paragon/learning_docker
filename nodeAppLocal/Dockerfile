FROM node:21-alpine3.18

RUN apk update \
    && apk upgrade \
    && apk add --no-cache bash

RUN mkdir node-starter && mkdir demo-storage

USER node

WORKDIR /node-starter

VOLUME /demo-storage

EXPOSE 4000

ENV NODE_ENV=dev 

CMD [ "npm", "start" ]