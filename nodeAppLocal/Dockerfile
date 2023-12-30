FROM node:21-alpine3.18

RUN apk update \
    && apk upgrade \
    && apk search git

RUN apk add git

RUN git clone https://github.com/pawas-saxena-paragon/node-starter.git

WORKDIR /node-starter

RUN npm install

EXPOSE 4000

ENV NODE_ENV=dev 

CMD [ "npm", "start" ]