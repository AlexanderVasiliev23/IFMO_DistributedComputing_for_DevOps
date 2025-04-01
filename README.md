# Развертывание Wordpress

## Используемые технологии

- База данных mysql
- Wordpress
- Docker с docker-compose
- Makefile
- Ansible

## Шаги для поднятия проекта

1. Предполагается, что в системе уже установлен ansible. Если нет - требуется его установить.
2. Создать файл inventory/host по примеру в [hosts.dist](inventory/hosts.dist)
3. Создать файл .env по примеру в [.env.dist](.env.dist)
4. В Makefile запустить target ```up-all``` . Команда в терминале: ```make up-all```

## Проверка результата

1. После поднятия проекта можно будет подключиться к базе данных по адресу "ip адрес сервиса:3306"
2. Можно будет перейти на сайт по адресу "ip адрес сервиса:8080"
   ![wordpress_is_working.png](wordpress_is_working.png)