Docker image with PHP, Composer, Node.js and NPM
===

Using php 7.4 cli, node.js 14.

### Pull it:

```bash
docker pull flamy/php-composer-node-npm
```

### Run it:

```bash
docker run --rm -it -v ${PWD}:/app -w /app flamy/php-composer-node-npm php helloworld.php
docker run --rm -it -v ${PWD}:/app -w /app -v composer-cacahe:/tmp flamy/php-composer-node-npm composer install
docker run --rm -it -v ${PWD}:/app -w /app flamy/php-composer-node-npm node helloworld.js
docker run --rm -it -v ${PWD}:/app -w /app flamy/php-composer-node-npm npm install
```

---
[Docker hub repository.](https://hub.docker.com/r/flamy/php-composer-node-npm)
