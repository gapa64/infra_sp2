# Квик старт

Проект **infra_sp2** разворачивает проект api_yamdb в контейнерах Docker.  
api_yamdb собирает отзывы пользователей на произведения

## Заупстить

```bash
git clone https://github.com/gapa64/infra_sp2
docker-compose up infra_sp2/infra/docker-compose.yaml 
```

### Миграции
```bash
python3 ./api_yamdb/manage.py makemigrations
python3 ./api_yamdb/manage.py migrate
```

### Запустить
```bash
python3 ./api_yamdb/manage.py runserver
```



### Полезные линки
[Модели на диаграммах](https://drive.google.com/file/d/1T9OHj-UAWXTzzAm7cWSml5KN8PDwlQUf/view?usp=sharing)  
Борда с тасками в [Проджектах](https://github.com/AlexPunches/api_yamdb/projects/2)

