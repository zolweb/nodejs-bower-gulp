# Use Alpine Linux
FROM alpine:3.4

# Declare maintainer
MAINTAINER Yannick PEREIRA-REIS <yannick.pereira.reis@gmail.com>

# Timezone
ENV TIMEZONE Europe/Paris

ENV NODE_VERSION 6.6.0
ENV NPM_VERSION 3.10.8

# Let's roll
RUN	apk update && \
	apk upgrade && \
	apk add --update tzdata sudo bash wget python python-dev make g++ git && \
	cp /usr/share/zoneinfo/${TIMEZONE} /etc/localtime && \
	echo "${TIMEZONE}" > /etc/timezone && \
	apk add --update nodejs && \
	npm install -g npm@"${NPM_VERSION}" bower gulp && \
	npm cache clean -f && \
	apk del tzdata && \
	mkdir /data && \
	rm -rf /var/cache/apk/*

WORKDIR /data

CMD ["bash"]
