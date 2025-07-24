FROM node:24
ARG NODE_MAJOR=24

RUN npm install -g typescript && npm install -g http-server && npm install -g start-server-and-test


#NB: xvfb and libglib-2.0.so is a required dependency of cypress
RUN apt-get update && \
  apt-get install --no-install-recommends -y \
  libgtk2.0-0 \
  libgtk-3-0 \
  libnotify-dev \
  libgconf-2-4 \
  libgbm-dev \
  libnss3 \
  libxss1 \
  libasound2 \
  libxtst6 \
  procps \
  xauth \
  xvfb

RUN npm install -g cypress


