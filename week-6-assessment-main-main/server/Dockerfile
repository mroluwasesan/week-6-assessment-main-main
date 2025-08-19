FROM node:17-alpine

ARG ATLAS_URI

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 5050

ENV ATLAS_URI=${ATLAS_URI}

CMD ["npm", "run", "start"]