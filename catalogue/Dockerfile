FROM node:node:20-alpine3.21 AS BUILDER
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install

FROM node:node:20-alpine3.21
RUN addgroup -S roboshop && adduser -S roboshop -G roboshop
ENV  MONGO="true"\
     MONGO_URL="mongodb://mongodb:27017/catalogue"
WORKDIR /opt/server
USER roboshop
COPY --FROM=BUILDER /opt/server /opt/server   
CMD ["node","server.js"]   
