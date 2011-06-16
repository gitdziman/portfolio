Движок портфолио web-студии stfalcon.com
========================================

Установка
---------

Очередность действий такая:

1. Копируем проект с репозитория.

2. В консоли идем в папку с проектом.

3. Запускаем `bin/vendors`. Этот скрипт автоматически загрузит все необходимые дополнительные библиотеки в папку vendor проекта (вместе с zf2).

4. В файлах `app/config/config.yml` и `app/config/config_dev.yml` меняем параметры коннекта к БД на свои:

5. В консоли набираем `./console doctrine:database:create` и `./console doctrine:migration:migrate` эти команды создают БД и накатывают на неё существующие миграции.