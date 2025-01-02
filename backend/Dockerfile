FROM node:16.19.0-alpine3.17

WORKDIR /app

RUN apk add --no-cache \
    python3 \
    make \
    g++ \
    gcc \
    musl-dev \
    postgresql-client 

COPY package*.json ./

RUN npm install

COPY . .

CMD [ "npm", "run", "start:dev" ]
