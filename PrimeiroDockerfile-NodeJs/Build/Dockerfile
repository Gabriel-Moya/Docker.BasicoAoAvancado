FROM node:17-alpine3.14

LABEL maintainer="Gabriel Moya"

RUN mkdir /var/node

WORKDIR /var/node

COPY app.js .

EXPOSE 3000

CMD ["node", "app.js"]
