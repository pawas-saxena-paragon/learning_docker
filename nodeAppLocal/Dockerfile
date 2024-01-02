FROM node:21-alpine3.18

RUN apk update \
    && apk upgrade \
    && apk search git \
    && apk add git \
    && apk add --no-cache bash

RUN git clone https://github.com/Bam92/node-starter.git

WORKDIR /node-starter

RUN npm install

EXPOSE 4000

CMD [ "npm", "start" ]