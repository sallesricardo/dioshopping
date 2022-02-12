FROM node:14-alpine

RUN apk add --no-cache --update make gcc g++ zip bash yarn

COPY . /opt/frontend
WORKDIR /opt/frontend
RUN yarn

CMD yarn build
