FROM node:18-alpine
WORKDIR /app

COPY package.json ./
COPY yarn.lock ./
RUN yarn install --production

EXPOSE 3000

# COPY ./src/ ./src/
# COPY ./spec/ ./spec/

COPY . .

CMD ["node", "src/index.js"]