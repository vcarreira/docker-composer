# Composer docker image for Laravel

This is a [Docker](http://www.docker.com) image for the [composer CLI](https://getcomposer.org/) suited to be used with the [Laravel PHP Framework](http://laravel.com/).

An automated build for this repo is available on the [Docker Hub](https://registry.hub.docker.com/u/vcarreira/composer/).

This image works well with the below related images.

  - [vcarreira/nginx-php5-fpm](https://registry.hub.docker.com/u/vcarreira/nginx-php5-fpm)
  - [vcarreira/artisan](https://registry.hub.docker.com/u/vcarreira/artisan)
  - [vcarreira/phpunit](https://registry.hub.docker.com/u/vcarreira/phpunit)
  - [vcarreira/phpspec](https://registry.hub.docker.com/u/vcarreira/phpspec)

## Running composer commands
The container working directory is the volume ```/var/www```. You can run any composer command like this:

```
docker run -t --rm -v $(pwd):/var/www vcarreira/composer <composer args here>
```

---

:ok_hand: Happy Coding. 

If you have any feedback or questions, feel free to contact me on Twitter with [@vcarreira](https://twitter.com/vcarreira) or email with [vitor.carreira@gmail.com](mailto:vitor.carreira@gmail.com).
