FROM node:16-bullseye

LABEL maintainer="me@codingoncatnip.de"

RUN echo fs.inotify.max_user_watches=524288 | tee -a /etc/sysctl.conf && sysctl -p
RUN curl -f https://get.pnpm.io/v6.16.js | node - add --global pnpm@6
RUN pnpm config set store-dir .pnpm-store