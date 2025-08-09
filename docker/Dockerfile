FROM node:21.5

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

RUN npx prisma generate

CMD ["npm", "run", "dev"]