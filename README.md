# Тестовое задание - Кондратьев Дмитрий Олегович
#### Моё резюме: https://kazan.hh.ru/resume/e5f933f2ff0d7ea3370039ed1f663175394c6f
- Почта: dimakond520@gmail.com
- Телефон: +79379948305
- Telegram - https://t.me/xpand3xxwqr1

## Быстрый старт
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
