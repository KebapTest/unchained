ARG NODE_VERSION
FROM node:${NODE_VERSION}
LABEL maintainer="hi@kenshi.io"
ARG UNCHAINED_VERSION

WORKDIR /app

COPY ./entrypoint.sh entrypoint.sh

RUN npm i -g @kenshi.io/unchained@$UNCHAINED_VERSION && \
    unchained --version

ENTRYPOINT ["./entrypoint.sh"]
