FROM node:24.14.1-alpine

WORKDIR /api

RUN corepack enable && corepack prepare pnpm@latest --activate

COPY package.json pnpm-lock.yaml ./

RUN pnpm install --frozen-lockfile --ignore-scripts 

CMD ["pnpm", "start:dev"]
