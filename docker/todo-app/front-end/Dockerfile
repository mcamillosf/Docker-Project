FROM node:14-alpine3.12
EXPOSE 3000

WORKDIR /app

ADD node_modules.tar.gz ./

COPY ["package.json", "package-lock.json*", "./"]
RUN npm install

COPY . .

CMD ["npm", "start"]