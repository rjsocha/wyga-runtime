# PHP

##  Supported tags

  7.4

  * wyga/php:7.4-apache
  * wyga/php:7.4-fpm
  * wyga/php:7.4-fpm-alpine

  8.0

  * wyga/php:8.0-apache
  * wyga/php:8.0-fpm
  * wyga/php:8.0-fpm-alpine

  8.1

  * wyga/php:8.1-apache
  * wyga/php:8.1-fpm
  * wyga/php:8.1-fpm-alpine

  8.2

  * wyga/php:8.2-apache
  * wyga/php:8.2-fpm
  * wyga/php:8.2-fpm-alpine

###  All versions are precompiled with following modules:

```
[PHP Modules]
bcmath
bz2
calendar
Core
ctype
curl
date
dom
exif
fileinfo
filter
ftp
gd
gettext
gmp
hash
iconv
intl
json
libxml
mbstring
mysqli
mysqlnd
openssl
pcre
PDO
pdo_mysql
pdo_pgsql
pdo_sqlite
pgsql
Phar
posix
readline
Reflection
session
SimpleXML
sodium
SPL
sqlite3
standard
tokenizer
xml
xmlreader
xmlwriter
Zend OPcache
zip
zlib

[Zend Modules]
Zend OPcache
```

###  Additional modules are precomipled but not enabled:

```
mcrypt
mongodb
memcache
memcached
redis
xdebug
```

They can be enabled via commands:
```
docker-php-ext-enable-mcrypt
docker-php-ext-enable-mongodb
docker-php-ext-enable-memcache
docker-php-ext-enable-memcached
docker-php-ext-enable-redis
docker-php-ext-enable-xdebug
```

or by using env-conf (docker compose example):
```
    environment:
      ENVCFG: '/usr/local/etc/php/conf.d/runtime.ini:ENEXT'
      ENEXT100: 'extension=mcrypt.so'
      ENEXT103: 'extension=memcache.so'
      ENEXT104: 'extension=memcached.so'
      ENEXT105: 'extension=redis.so'
      ENEXT106: 'extension=mongodb.so'
      ENEXT999: 'zend_extension=xdebug.so'
```

# nginx

## Supported tags

  * wyga/nginx:1.23.2-alpine wyga/nginx:1.23-alpine wyga/nginx:mainline-alpine
  * wyga/nginx:1.22.2-alpine wyga/nginx:1.22-alpine wyga/nginx:stable-alpine wyga/nginx:alpine

