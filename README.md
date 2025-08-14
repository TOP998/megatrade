# MegaTrade — Static Site for Render

Готовый статический сайт с файлом `index.html` в корне. Можно сразу загружать на Render.

## 🚀 Как загрузить на Render

1. Создайте **публичный** репозиторий на GitHub, например `megatrade-site`.
2. В этой папке выполните команды:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<ВАШ_ЛОГИН>/megatrade-site.git
git push -u origin main
```

3. Зайдите на https://render.com → **New +** → **Static Site**.
4. Выберите ваш репозиторий.
5. Настройки:
   - **Build Command**: *(оставьте пустым)*
   - **Publish Directory**: `.`
   - **Branch**: `main`
6. Нажмите **Create Static Site** и дождитесь публикации.

### ⚙ Если есть роутинг (SPA)
В настройках Render → **Redirects/Rewrites** добавьте:
- Source: `/*`
- Destination: `/index.html`
- Type: `200`

Готово! Ваш сайт будет доступен по ссылке Render.