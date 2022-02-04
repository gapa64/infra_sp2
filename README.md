# Квик старт

Проект **infra_sp2** разворачивает проект api_yamdb в контейнерах Docker.  
api_yamdb собирает отзывы пользователей на произведения

## Заупстить

```bash
git clone https://github.com/gapa64/infra_sp2
docker-compose -f infra_sp2/infra/docker-compose.yaml up
```

### Шаблон env
```bash
DB_ENGINE=django.db.backends.postgresql
DB_NAME=postgres
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
DB_HOST=db
DB_PORT=5432
```

### Некоторые полезные команды
```bash
docker-compose exec web python manage.py migrate 
Применить миграции

docker-compose exec web python manage.py createsuperuser 
Создать супер пользователя Django

docker-compose exec web python manage.py collectstatic --no-input 
Cобрать статику

docker-compose exec web python manage.py loaddata fixtures.json
Загрузить тестовые данные
```

### Полезные линки
```bash
Docker image проекта api_yamdb  gaps64/api_yamdb:v2.4
```

## Автор
- [Sergey K](https://github.com/gapa64)