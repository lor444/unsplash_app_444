FROM node:8-alpine

LABEL maintainer="Alvise Susmel <alvise@poeticoding.com>"

WORKDIR /app


ADD package-lock.json ./package-lock.json
ADD package.json ./package.json
RUN npm install 

ADD ./app.js app.js
ADD ./views views


EXPOSE 3000/tcp
ENV NODE_ENV production 


CMD ["node", "app.js"]