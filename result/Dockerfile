# Shared base
FROM node:18-slim AS base

WORKDIR /app

COPY package*.json ./

RUN npm ci \
 && npm cache clean --force \
 && mv /app/node_modules /node_modules

COPY . .

ENV PORT 80

EXPOSE 80

CMD ["node", "server.js"]

# Development
FROM base as dev

RUN npm install -g nodemon

# Production
FROM base
