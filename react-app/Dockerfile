FROM node:14.16.0-alpine3.13
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /react-app
COPY . .
RUN npm install
ENV API_URL=http://my.app.url
EXPOSE 3000
CMD ["npm","start"]
