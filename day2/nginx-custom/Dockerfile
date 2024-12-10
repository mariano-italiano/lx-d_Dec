FROM alpine:3.21.0 AS helper-clone
RUN apk add git --no-cache
WORKDIR /src
ARG BRANCH_NAME=master
RUN git clone https://github.com/mariano-italiano/lx-d_Dec.git && cd lx-d_Dec && git checkout $BRANCH_NAME

FROM nginx:1.19.2
LABEL "author"="Marcin Kuajwski"
LABEL "version"="draft version"
RUN apt-get update && apt-get clean && rm -rf /var/lib/apt/lists/*
COPY --from=helper-clone /src/lx-d_Dec/index.html /usr/share/nginx/html/index.html
