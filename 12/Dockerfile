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
    python 

# Setup working directory
WORKDIR /var/www