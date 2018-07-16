# README

## Setup

```
$ docker-compose up -d
$ docker-compose exec web bash
$ rails new . --database=postgresql
```

Edit database.yml

```
  host: db
  username: postgres
  password: postgres
```

```
$ rails db:migrate
```
