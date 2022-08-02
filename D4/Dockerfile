FROM node:latest

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install
# Run npm ci --only=production
# use the above one if working in production

COPY . .

# expose port to host
EXPOSE 8080

CMD [ "node", "server.js" ]