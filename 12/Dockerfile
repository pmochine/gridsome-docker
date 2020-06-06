FROM node:12-alpine

# Install build tools
# Needed by npm install
RUN apk update && apk upgrade
RUN apk --no-cache add --virtual native-deps \
    git \
    g++ \
    gcc \
    libgcc \
    libstdc++ \
    linux-headers \
    make \
    python \
    openssh-client \
    util-linux \
    libtool \
    bash \
    libpng-dev \
    zlib-dev

# Setup working directory
WORKDIR /var/www