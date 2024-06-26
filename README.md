symfony-http-client-ext
--

Functions to solve most Symfony HttpClient problems. 

How to use
---
Create a class with the getHttpClient method, example: src/ExampleClass.php

Tests
------------
```sh
docker build -t yapro/symfony-http-client-ext:latest -f ./Dockerfile ./
docker run --rm -v $(pwd):/app yapro/symfony-http-client-ext:latest bash -c "cd /app \
  && composer install --optimize-autoloader --no-scripts --no-interaction \
  && /app/vendor/bin/phpunit /app/tests"
```

Dev
------------
```sh
docker build -t yapro/symfony-http-client-ext:latest -f ./Dockerfile ./
docker run -it --rm -v $(pwd):/app -w /app yapro/symfony-http-client-ext:latest bash
composer install -o
```
