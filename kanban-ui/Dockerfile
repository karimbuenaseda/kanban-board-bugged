FROM node:12.7-alpine

WORKDIR /usr/src/app

COPY package.json ./
RUN npm config rm proxy
RUN npm config rm https-proxy
RUN npm install

COPY . .

EXPOSE 4200

CMD ["npm", "start"]