FROM node:9-alpine
RUN apk add --update tini
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install && npm cache verify
COPY . .
ENV PORT 8080
EXPOSE 8080
CMD [ "npm", "start" ]
