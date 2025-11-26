# Тестовое задание - Кондратьев Дмитрий Олегович
#### Моё резюме: https://kazan.hh.ru/resume/e5f933f2ff0d7ea3370039ed1f663175394c6f
#### ТЗ: https://docs.google.com/document/d/16fR8yRFT8uSrpWAf6mvVJxAH4jnbgjbSaJQcC9CP8NE
- Почта: dimakond520@gmail.com
- Телефон: +79379948305
- Telegram - https://t.me/xpand3xxwqr1

# ✨ Информация
- URL фронтенда - http://localhost:3000
- URL бекенда (API) - https://localhost:8000, с эндпоинтом GET /items - https://localhost:8000/items
#### Оптимизации:
- Индекс на таблице `item(created_at)` для оптимизированной выдачи с сортировкой по `created_at`
- Кэширование (in-memory) на уровне приложения Nest.JS с помощью `CacheInterceptor`
- Пагинация для запроса `item` с LIMIT (по умолчанию 20), OFFSET
- DB Connection Pool оптимизация осуществляется автоматически с помощью Nest.JS, один раз создается соединение и через Dependency Injection доставляется в нужные сервисы
#### Потенциально можно добавить запуск подпроцессов через `cluster`, чтобы нагрузка распределялась по инстанциям (round-robin на linux, по нагрузке на windows). 
#### Так же можно сделать на уровне nginx, запустив при этом несколько серверов.
#### В результате получаем легкое масштабирование и высокую производительность.

# 🚀 Быстрый старт
```bash
git clone https://github.com/wqr11/demo.git &&\
cd demo &&\
git submodule init &&\
git submodule update --recursive --remote &&\
cp demo-backend/.env.example demo-backend/.env &&\
cp demo-frontend/.env.example demo-frontend/.env &&\
docker compose up --build
```

## ⚙ Команды в отдельности 
### 1) Склонируйте репозиторий и инициализируйте подмодули
```bash
git clone https://github.com/wqr11/demo.git &&\
cd demo &&\
git submodule init &&\
git submodule update --recursive --remote
```

### 2) Скопируйте содержимое .env.example в файл .env внутри модулей
```bash
cp demo-backend/.env.example demo-backend/.env &&\
cp demo-frontend/.env.example demo-frontend/.env
```

### 3) Запустите docker compose
```bash
docker compose up --build
```
