# Custom docker images

multi purpose images, mostly used for local development

## PHP

Docker Hub name: **trivaldock/php**

this image enables serving of a php directory with an apache server. based on the official php:apache image, but enables more php extensions and mods, so that php application can be served out of the box.
Inspired by existing Wordpress and Grav images.

Usage example:

```
docker run -d --rm -p 8000:80 --name myphp -v "$PWD":/var/www/html trivaldock/php
```
