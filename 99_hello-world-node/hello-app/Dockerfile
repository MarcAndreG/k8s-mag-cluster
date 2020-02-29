FROM node:13 as Dev

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install --only=development

COPY . .

RUN npm run build

FROM node:13 as Prod

COPY package*.json ./

RUN npm install --only=production

COPY . .

COPY --from=Dev /usr/src/app/dist ./dist

CMD ["node", "dist/main"]