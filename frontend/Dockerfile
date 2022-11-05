FROM node:18-alpine

WORKDIR /app

# Copy source code to working directory
COPY package.json ./

RUN npm install

COPY . .

RUN npm run build 

EXPOSE 3000

CMD ["npx", "serve", "build"]