FROM node:14

RUN npm install @angular/cli@11.0.0 -g

WORKDIR /app
COPY package.json .
COPY package-lock.json .
RUN npm install
COPY . .
ENV PATH /app/node_modules/.bin:$PATH
