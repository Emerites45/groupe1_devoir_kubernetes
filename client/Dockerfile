FROM node:alpine

ENV CI=true
ENV WDS_SOCKET_PORT=0

WORKDIR /app
COPY package.json ./
COPY ./ ./
EXPOSE 3000
CMD ["npm", "start"]
