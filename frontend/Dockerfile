FROM node:24.3.0-slim

WORKDIR /app

COPY ./package*.json /app/

RUN npm ci

COPY .. .

RUN npm run build

CMD ["node", ".output/server/index.mjs"]
