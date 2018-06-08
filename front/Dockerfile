FROM node:10.4.0

COPY package.json package-lock.json elm-package.json /usr/src/app/

WORKDIR /usr/src/app

RUN set -x \
  && npm install \
  && npm run elm-install

COPY . ./

CMD ["npm", "run", "start"]

EXPOSE 8080
