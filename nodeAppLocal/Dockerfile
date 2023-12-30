FROM node:21-alpine3.18

RUN apk update \
    && apk upgrade

RUN mkdir node-starter

RUN cd /node-starter && pwd

WORKDIR /node-starter

EXPOSE 4000

ENV NODE_ENV=dev 

CMD [ "npm", "start" ]