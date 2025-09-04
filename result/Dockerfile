# Shared base
FROM node:18-alpine

WORKDIR /app

COPY . .

RUN npm config set registry https://registry.npmjs.org \
 && npm install -g nodemon

RUN npm install \
 && npm cache clean --force \
 && mv /app/node_modules /node_modules

ENV PORT=80

EXPOSE 80

CMD ["node", "server.js"]
