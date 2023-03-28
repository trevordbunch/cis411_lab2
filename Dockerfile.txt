FROM node:15
WORKDIR /dist
COPY package.json /dist
RUN npm uninstall graphql
RUN npm install express express-graphql
RUN npm install graphql
COPY . /dist
CMD node server.js
EXPOSE 4000