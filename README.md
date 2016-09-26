## Docker image with nodejs, npm, bower and gulp

| Tool | Version |
|------|---------|
| Nodejs | v6.2.0 |
| Npm | 3.10.8 |
| Bower | 1.7.9 |
| Gulp | [12:56:31] CLI version 3.9.1 |


### Base Docker Image

* [Dockerhub Alpine 3.4](https://hub.docker.com/_/alpine/)
* [Github](https://github.com/gliderlabs/docker-alpine/tree/8f23fc2e995ab8f7f0f5960c6a1ddd12f57efd0c/versions/library-3.4)


### Installation

```
docker pull zolweb/nodejs-bower-gulp:alpine-node_6.6.0-npm_3.10.8
```

### Usage

#### Run `node`

```
$ docker run -it --rm zolweb/nodejs-bower-gulp:alpine-node_6.6.0-npm_3.10.8 node -v
v6.2.0
```

#### Run `npm`

```
$ docker run -it --rm zolweb/nodejs-bower-gulp:alpine-node_6.6.0-npm_3.10.8 npm -v
3.10.8
```

#### Run `bower`

```
$ docker run -it --rm zolweb/nodejs-bower-gulp:alpine-node_6.6.0-npm_3.10.8 bower -v
1.7.9
```

#### Run `gulp`

```
$ docker run -it --rm zolweb/nodejs-bower-gulp:alpine-node_6.6.0-npm_3.10.8 gulp -v
[12:56:31] CLI version 3.9.1
```
