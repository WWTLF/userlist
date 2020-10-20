# Otus 1.6 Homework

- [x] PostgreSQL подключен как зависимость
- [x] Геренрируется 2 Job'а:
  - create-user-job -  создает нового пользователя Postgres с ограниченными правами
  - userlist-migrate Производит миграцию данных с помощью инстурмента https://github.com/golang-migrate/migrate, исходный код контейнера миграции тут: https://github.com/WWTLF/otus/tree/master/userlist-migration-src
- [x] Главный сервис userlist https://github.com/WWTLF/otus/tree/master/user-list-src
- [x] Пароли лежат в secrets


## Установка

```
helm repo add wwtlf https://wwtlf.github.io/userlist
helm repo update
helm install otus userlist -f values.yaml  
```
