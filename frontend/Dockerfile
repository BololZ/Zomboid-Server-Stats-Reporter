FROM node:lts-alpine
WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install && npm cache clean --force
# Bundle app source
COPY . .

EXPOSE 3000

CMD ["npm", "start"]