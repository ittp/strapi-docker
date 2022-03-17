FROM strapi/base

WORKDIR /api1

COPY ./package.json ./
COPY ./yarn.lock ./

RUN yarn install

COPY . .

ENV NODE_ENV development

RUN yarn build

EXPOSE 2337

CMD ["yarn", "develop"]
