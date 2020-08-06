# pappz-laravel-docker
# Simple docker for laravel

- docker-compose exec app bash

- in terminal you can do everything like
 - composer create-project --prefer-dist laravel/laravel .




---------------------------------------

### APP start or update

docker exec -it AGROHOF_app bash

git pull

composer install

php artisan migrate

run:
php artisan db:seed --class=PermissionsTableSeeder
php artisan db:seed --class=PermissionRoleTableSeeder
---------------------------------------

--------------------------------------
### TO RESTORE MYSQL DB IN CONTAINER MYSQL

place mysql backup (.sql ) file to ./mysql-backup folder

### enter dataase container with the following command:
docker exec -it AGROHOF_database bash

### when you are in, run the following commands:
- cd /home/mysql-backup

- mysql -u root -p $MYSQL_DATABASE < SQLFILENAME-which-YOU-put.sql

- enter root password
---------------------------------------

### Run Node container
docker exec -it AGROHOF_app bash

run the basic npm commands

npm run watch
npm run dev
npm run prod

