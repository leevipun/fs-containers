FROM node:24

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm ci

COPY . .

ENV port=3000

CMD ["npm", "run", "dev"]

## docker run --rm --name todo-backend -p 3000:3000 todo-backend