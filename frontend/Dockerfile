FROM node:18-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install -g live-server
RUN npm install

COPY . .

EXPOSE 3000

CMD ["live-server", "--host=0.0.0.0", "--port=3000", "--no-browser"]
