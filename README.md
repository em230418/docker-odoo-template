# docker-odoo

## Команды

Запуск Odoo

```
docker-compose up odoo
```

Пересборка образов (применяется после редактирования Dockerfile)

```
docker-compose build
```

Запуск Odoo с пересборкой образов

```
docker-compose up odoo --build
```

Запуск Odoo shell

```
docker-compose run odoo odoo shell -d dbname
```

Прямой доступ к БД посредством утилиты psql

```
PGPASSWORD=odoo psql -h localhost -p 5433 postgres odoo
# далее, чтобы переключиться к базе вводим
# \c dbname
```

## Адреса

- [http://odoo.localhost](http://odoo.localhost) - сам Odoo
- [http://mail.localhost](http://mail.localhost) - фейковая почта
- [http://wdb.localhost](http://wdb.localhost) - отладчик
