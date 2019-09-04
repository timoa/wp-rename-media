# WIP - Wordpress Rename Media

PHP script that search for media files with special characters, rename them, update the DB and create an 301 redirection to avoid to lose your SEO.

I'm developing this PHP script for a client to automatically rename years of special characters in the filename

I will try to make it generic but let me know if it doesn't work for you.

Warning: This project is in progress!

## Test

To test this script, I started to use Docker with the following images:

* Wordpress (latest)
* MySQL (5.7)
* phpMyAdmin (latest)

The goal is to seed MySQL with a basic Wordpress install and dummy data (media with special characters and Posts linked to them).

To launch the current configuration, just run:

``` bash
cd test
docker-compose up
```

### URL

| Image | URL | Login | Password |
|---|---|---|---|
| Wordpress | <http://localhost:8000> | | |
| phpMyAdmin | <http://localhost:8080> | `wordpress` | `wordpress` |

[wordpress-url]: http://localhost:8000
[phpmyadmin-url]: http://localhost:8080
