# adopted from https://pnpm.io/docker#example-2-build-multiple-docker-images-in-a-monorepo

# using non-slim, for "production debugging"
FROM node:24 AS base
ENV PNPM_HOME="/pnpm"
ENV CI=true
ENV PATH="$PNPM_HOME:$PATH"
RUN corepack enable

FROM base AS build
COPY . /usr/src/app
WORKDIR /usr/src/app
RUN --mount=type=cache,id=pnpm,target=/pnpm/store pnpm install --frozen-lockfile
RUN pnpm run -r build
RUN pnpm deploy --filter=web --prod /prod/web


FROM base AS web
COPY --from=build /prod/web /app
WORKDIR /app
EXPOSE 4321
ENV HOST=0.0.0.0
CMD [ "node", "./dist/server/entry.mjs" ]