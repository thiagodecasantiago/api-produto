FROM node:14.16.1-alpine3.13
USER node
RUN mkdir -p /home/node/api-produto
WORKDIR /home/node/api-produto
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD [ "node", "app.js" ]