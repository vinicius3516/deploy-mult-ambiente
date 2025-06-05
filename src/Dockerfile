FROM node:23-alpine3.20
RUN adduser -D -h /home/appuser appuser
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
USER appuser
EXPOSE 8080
CMD [ "node", "server.js" ]
