# Stock calc

then prepare docker environment:
```
docker compose build
docker compose up -d
docker compose run php bash
```

final project steps inside of docker container:
```
composer install
bin/console doctrine:database:create
bin/console doctrine:schema:create
```


```
docker exec -it  stock_calc_php bash
./vendor/bin/phpunit --colors --verbose --testdox
```