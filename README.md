Docker image with PHP, Composer, Node.js and NPM
===

Using php 7.3 cli, node.js 12

### Pull it:
```
docker pull flamy/php-composer-node-npm
```

### Run it
```
docker run --rm -it -v ${PWD}:/app -w /app flamy/php-composer-node-npm php helloworld.php
docker run --rm -it -v ${PWD}:/app -w /app -v composer-cacahe:/tmp flamy/php-composer-node-npm composer install
docker run --rm -it -v ${PWD}:/app -w /app flamy/php-composer-node-npm node helloworld.js
docker run --rm -it -v ${PWD}:/app -w /app flamy/php-composer-node-npm npm install
```

---
Docker hub repository: https://hub.docker.com/r/flamy/php-composer-node-npm
