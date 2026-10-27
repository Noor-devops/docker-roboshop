FROM node:20.20.2-alpine3.22 As builder
WORKDIR /app
COPY package*.json .
COPY *.js .
RUN npm install

FROM node:20.20.2-alpine3.22
WORKDIR /app
EXPOSE 8080
COPY --from=builder /app /app
CMD ["node", "server.js"]


# FROM node:20.20.2-alpine3.22
# WORKDIR /app
# COPY package*.json .
# COPY *.js .
# RUN npm install
# CMD ["node", "server.js"]