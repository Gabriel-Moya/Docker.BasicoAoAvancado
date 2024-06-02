FROM node:17-alpine3.14

LABEL maintainer="Gabriel Moya"

VOLUME [ "/var/nodeapp" ]

RUN adduser -h /var/nodeapp -s /bin/bash -D nodeapp

WORKDIR /var/node

COPY app.js .
RUN chown nodeapp:nodeapp app.js

EXPOSE 3000

ARG VERSION
ENV VERSION=${VERSION:-1.0.0}

USER nodeapp
CMD ["node", "app.js"]
