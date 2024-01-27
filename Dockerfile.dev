FROM node:20.11-alpine3.18 AS base

WORKDIR /app

COPY package.json  ./

COPY pnpm-lock.yaml* ./

RUN npm install -g pnpm@8.9

RUN pnpm install --frozen-lockfile

COPY . .

EXPOSE 5173

CMD ["pnpm", "run", "dev"]

