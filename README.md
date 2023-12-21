# PHP Ecosystem Multi-Framework Docker Repository

Welcome to the PHP Ecosystem Multi-Framework Docker Repository! 🚀

Unleash the full potential of your PHP development with our versatile Docker image. This repository offers seamless support for popular frameworks like Laravel, Symfony, Slim, CodeIgniter, Yii, and more. Linked with [GitHub](https://github.com/nanorocks/php-ecosystem-multi-framework) and inspired by this [repo](https://github.com/sports-match-maker/docker-pnmamhes), our unified environment provides efficiency and ease of use.

**Note: Currently, all frameworks support PHP 8.2.** The repository is equipped with MySQL and PostgreSQL support, ensuring compatibility with diverse database choices. Additionally, necessary PHP extensions are preconfigured for each framework, streamlining your development process.

Dive into a user-friendly PHP setup, accelerating your projects effortlessly. Explore our overview guide for insights on running and maximizing the capabilities of this dynamic Docker image. Happy coding with the PHP Ecosystem Multi-Framework image for Docker!

Example docker-compose.yml for php-ecosystem-multi-framework:
```
version: '3.1'

services:
  php-fpm:
    image: nanorocks/php-ecosystem-multi-framework
    container_name: php-fpm
    volumes:
      - ./src/laravel:/var/www/html/laravel
      - ./src/symfony:/var/www/html/symfony
      - ./src/codeigniter:/var/www/html/codeigniter
      - ./src/slim:/var/www/html/slim
      - ./src/yii:/var/www/html/yii
    networks:
      - docker-pnmamhes
```

Reference: [Here](https://github.com/sports-match-maker/docker-pnmamhes)
