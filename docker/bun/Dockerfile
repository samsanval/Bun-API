FROM oven/bun

WORKDIR /home/app

COPY package.json .
COPY bun.lockb .

RUN bun install

COPY tsconfig.json .
# COPY public public

ENV NODE_ENV production
CMD ["bun", "src/index.ts"]

EXPOSE 3000