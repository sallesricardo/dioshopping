FROM node:14-alpine

RUN mkdir /opt/backend
WORKDIR /opt/backend
COPY . /opt/backend

RUN apk add --no-cache make gcc g++ tzdata bash yarn
RUN cp /usr/share/zoneinfo/Brazil/East /etc/localtime
RUN echo "Brazil/East" > /etc/timezone

RUN yarn

EXPOSE 3000

CMD yarn start