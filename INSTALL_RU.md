# Деплой Void Node Website через GitHub → Render

## 1. GitHub
1. Открой https://github.com/new
2. Создай репозиторий, например `VoidNode-Website`.
3. Можно сделать Public.
4. Не добавляй секреты, API keys или `.env`.
5. Загрузи содержимое этой папки в корень репозитория: `index.html` не обязателен для Render, но страницы RU/EN лежат в `ru/` и `en/`.

## 2. Render
1. Открой https://dashboard.render.com/
2. `New` → `Static Site`.
3. Подключи GitHub и выбери `VoidNode-Website`.
4. Branch: `main`.
5. Build Command: оставить пустым.
6. Publish Directory: `.`.
7. Create Static Site.

Render автоматически будет передеплоить сайт после push в подключённую ветку.

## 3. Адрес
После деплоя Render выдаст адрес вида `https://<name>.onrender.com`.

## 4. Языки
Русская версия: `/ru/`
Английская версия: `/en/`

## 5. Важно
Регион Ohio относится к backend-сервису Void Node. Static Site на Render обслуживается глобальным CDN и отдельный регион для него не выбирается.
