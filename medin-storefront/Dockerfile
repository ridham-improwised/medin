FROM improwised/docker-nodejs-base:18-latest

COPY package*.json /app

RUN npm install

RUN apk add git

COPY .env.example .env

COPY . /app

CMD [ "npm", "run", "dev" ]
