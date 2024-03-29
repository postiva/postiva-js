FROM node:20.11.0 as base
RUN npm install -g pnpm

FROM base AS pruner
WORKDIR /app
RUN npm install turbo -g
COPY . .
RUN turbo prune --scope=@postiva/docs --docker

FROM base AS installer
WORKDIR /app
COPY --from=pruner /app/out/json/ .
COPY --from=pruner /app/out/pnpm-lock.yaml ./pnpm-lock.yaml
RUN pnpm install --frozen-lockfile

FROM base AS builder
WORKDIR /app
COPY --from=installer /app/ .
COPY --from=pruner /app/out/full/ .
RUN pnpm docs:build

FROM base AS runner
WORKDIR /app
COPY --from=builder /app/ .
CMD pnpm docs:preview
