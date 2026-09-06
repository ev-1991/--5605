# KazIOR CRM v14 — GitHub Pages DEMO

Это специальная временная сборка для показа через GitHub Pages.

## Важно
В этой DEMO-сборке GREEN-API Token встроен в `app.js`.
Любой посетитель сайта может увидеть его через исходный код/DevTools.
После демонстрации обязательно замените токен.

## Загрузка
1. Создайте отдельный репозиторий, например `kazior-crm-demo`.
2. Загрузите содержимое этой папки в корень репозитория.
3. GitHub → Settings → Pages.
4. Source: `Deploy from a branch`.
5. Branch: `main`.
6. Folder: `/(root)`.
7. Save.

Адрес будет примерно:
`https://ВАШ_ЛОГИН.github.io/kazior-crm-demo/`

## Через Git
```bash
git init
git branch -M main
git add .
git commit -m "Temporary KazIOR CRM demo"
git remote add origin https://github.com/ВАШ_ЛОГИН/kazior-crm-demo.git
git push -u origin main
```

## После показа
GitHub → Repository → Settings → Pages → Unpublish site.

Затем:
- заменить GREEN-API Token;
- удалить demo-репозиторий/ветку;
- для постоянной публикации использовать SAFE BACKEND версию.

Если GREEN-API запросы будут блокироваться браузером/CORS, GitHub Pages это не исправит — тогда нужен Node.js backend/VPS.
