ARG version=20
FROM node:${version}
# this creates /app and move there
WORKDIR /app
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
COPY package.json .
COPY *.js
RUN npm install
CMD ["node","server.js"]