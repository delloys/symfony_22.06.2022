# symfony_22.06.2022




symfony.com download установить ччерез композер, по ссылке
cd /var/www/html
composer create-project symfony/skeleton:"6.1.*" zavod_project

если ок, то прриветств.сообщ.
whats next?
cd zavod_project
git init
git status
vim /etc/nginx/sites-enabled default

server{
..
root /var/www/html/zavod_project/public
} (картинка)

![1](https://user-images.githubusercontent.com/52314995/175464252-cdd31ea9-ce77-4d1f-860d-7e897ef302cd.jpg)

symfony nginx how to - symfony nginx 2 ссылка

nginx -s reload
(service nginx start)
service mnginx status
стартовая страница симфони, если все ок(красивенькая)

comment:
- id
- userID
- content
- createdAt
User:
- username
- id
- password*

symfony maker bundle 
composer require --dev symfony/maker-bundle
bin/console

bin/console make:contoller
homeController
less src/Controller/homeController.php

composer reqire twig

rm src../homecontroller.php

сделать заново контроллер
less templates/home/HomeCOntroller

#Route '/' редактировать распоожение

composer require orm
(object relatonal mapping)
доктрина???шо это doctrine
n
(если ок whats next)

vim .env (в корне проекта ?)
(картинка)

чо расскоментировать какую бд

bin/console make:entity
user
(создались файлы)
Поля(id не надо, доктрина сделает сама):
username
string
32
no

password
no
40
no

createdAt
datetime_immutabel
no

rm src/repository/userRepository 
cmposer require ?
bin/console make:user


username

bin/console make:migration
bin/console doctrine:migrations:migrate
(картинка)
bin/console make:entity
comment
content
text
no

createdAt
datetime_immu..
no

user
relation
user
ManyToOne
no
yes
comments
yes

less /src/Entity/Comment.php | User.php
(картинка)

bin/console make:crud
composer require form validator annotations
bin/console make:crud

user
userContorller
no

bin/console make:crud
comment
commentCOntroller
no

php bin/console make:migratiom
php bin/console doctrine:migrations:migrate
less src/Controller/UserController
ip/user/
будет ошибка 

vim src/Form/UserType.php
killdd(roles)
chmod 777 /var/data.db

symfony.som -> users

ip/comment/
vim /src/Entity/USer.php


public func __toString():string
{
  return $this->
  (картинка)
}

vim /src/Entity/comm

public func __construct()
{
картинка
$

}kill--> createdAt в src/Form/CommentType

vim src/contr/com/com.php
вставить откуда-то из другого контроллера
из HomeController
в HomeCOntroller (картинка)
дальше лень
см.запись

