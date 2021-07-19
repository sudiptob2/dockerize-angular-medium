FROM node:14

RUN npm install @angular/cli@11.0.0 -g

# Create and define the node_modules's cache directory.
WORKDIR /cache

COPY package.json .
COPY package-lock.json .
RUN npm install

# define the application's working directory.
WORKDIR /app
COPY . .
ENV PATH /app/node_modules/.bin:$PATH
