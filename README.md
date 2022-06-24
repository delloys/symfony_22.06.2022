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
![2](https://user-images.githubusercontent.com/52314995/175464323-abfcb939-bc8c-4bf6-ba48-5b179b067e27.jpg)


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
(картинка) (хз, эта или нет))
![3](https://user-images.githubusercontent.com/52314995/175464513-6ec2e3fa-3b3a-46e5-9048-d0ed7b811346.jpg)

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
![4](https://user-images.githubusercontent.com/52314995/175464562-9a7dcbdc-324a-4ca2-ba82-11ff167338a7.jpg)

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
(картинка) ??
![5](https://user-images.githubusercontent.com/52314995/175464606-dac847f3-2c86-457a-9051-9bb0e2bc12e7.jpg)
![6](https://user-images.githubusercontent.com/52314995/175464654-cb060d97-3be9-48f2-ad90-c03aa5f59375.jpg)

![7](https://user-images.githubusercontent.com/52314995/175464682-e3b5eb26-8750-478f-a360-016c520b39ac.jpg)


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
  ![8](https://user-images.githubusercontent.com/52314995/175464698-a9bbba15-a222-4c5b-9a32-63c9526979e5.jpg)
![9](https://user-images.githubusercontent.com/52314995/175464734-a7ee39cf-817e-4920-a886-d67c2d0aecd5.jpg)
![10](https://user-images.githubusercontent.com/52314995/175464749-28675622-0353-4d6e-adab-e0832dc519a8.jpg)

}

vim /src/Entity/comm

public func __construct()
{
картинка
![11](https://user-images.githubusercontent.com/52314995/175464763-7dd9f224-5d7a-4d44-a11c-3323f7fb6239.jpg)
![_11](https://user-images.githubusercontent.com/52314995/175464800-eab701b6-0d5c-4a33-935d-90b9e326d76f.jpg)

$

}kill--> createdAt в src/Form/CommentType

vim src/contr/com/com.php
вставить откуда-то из другого контроллера
из HomeController
в HomeCOntroller (картинка)
![_12](https://user-images.githubusercontent.com/52314995/175464817-a68738de-1fd3-444e-906f-50e47aab4912.jpg)
![_13](https://user-images.githubusercontent.com/52314995/175464836-5ce796bf-3710-4d2d-bffb-decaaa7ebfe6.jpg)
![_14](https://user-images.githubusercontent.com/52314995/175464843-03174fa4-5cdf-403f-a243-5d075c6194c2.jpg)
![_16](https://user-images.githubusercontent.com/52314995/175464875-4dff4e8b-d55a-4eac-91be-c7db645d740b.jpg)
![_17](https://user-images.githubusercontent.com/52314995/175464878-4ced5c60-7a7f-49e8-92f8-5270e9e55929.jpg)
![_18](https://user-images.githubusercontent.com/52314995/175464880-8d9e4855-03c2-49ba-be56-6dc0fb83c63e.jpg)


дальше лень
см.запись

