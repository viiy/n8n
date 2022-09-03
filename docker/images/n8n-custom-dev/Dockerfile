ARG NODE_VERSION=16

# 1. Create an image to build n8n
FROM node:${NODE_VERSION}-alpine
WORKDIR /app

RUN \
	apk --no-cache add git && \
	npm install -g run-script-os turbo

RUN npm config set legacy-peer-deps true
USER 1000
#	apk --no-cache add git && \
#	npm install -g run-script-os turbo

#COPY turbo.json package.json package-lock.json ./

#RUN chown -R 1000:1000 .
#RUN npm config set legacy-peer-deps true
#RUN sudo chown -R 1000:1000 "/home/node/.npm"

#USER node

#RUN \
#	npm ci && \
#  npm install && \
#  npm run dev

#ENV NODE_ENV=production
