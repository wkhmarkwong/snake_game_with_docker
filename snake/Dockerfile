FROM node:16-alpine

WORKDIR /snake

# copy package file first to optimize build time
COPY package.json .

RUN npm i

COPY . .

EXPOSE 19006

CMD ["npx", "expo", "start", "--web"]