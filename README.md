# moa

<img src="http://i.imgur.com/Ye2AO9J.png" alt="Redis" />

Please note that by default the cache is using plain old file cache. If you want to use Redis, change the configuration on line 18 of `api/app/config/cache.php` from `file` to `redis`. More information on the cache configuration is available on http://laravel.com/docs/cache#configuration.

#### info ####
http://habrahabr.ru/post/178525/
http://habrahabr.ru/post/64917/

Clear cache
$ redis-cli
$redis> flushall
OK
$redis> exit

Redis Desktop
/var/www/Magento-on-Angular/moa-api.com/api/vendor/monolog/monolog/src/Monolog/Handler/RedisHandler.php

host: localhost
name: application
port: 6379

https://github.com/uglide/RedisDesktopManager

#### Using console ####

1. Download Debian Package from  [http://redisdesktop.com/download](http://redisdesktop.com/download)
2. Install package:
    `dpkg -i redis-desktop-manager_X.X.X_i386.deb && apt-get -f install`
4. Run RedisDesktopManager :
	`/usr/share/redis-desktop-manager/bin/rdm`