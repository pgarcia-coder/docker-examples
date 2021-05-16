FROM alpine

RUN apk add --update nodejs-npm

WORKDIR /app

COPY package*.json ./

RUN npm ci

COPY . .

EXPOSE 8080

CMD ["npm", "start"]