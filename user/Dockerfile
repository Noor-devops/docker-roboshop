FROM node:20.20.2-alpine3.22
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
EXPOSE 8080
CMD ["node", "server.js"]