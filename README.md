# python-actions-mkdons

morecambe демонстрирует создание собственного сайта на базе **MkDocs** с использованием:
- Кастомной темы на **Jinja2** (header, footer, стилизация страниц)
- Сборки фронтенда (PostCSS, autoprefixer)
- Валидации и минификации HTML
- Автоматической публикации на **GitHub Pages**

## ⚙️ Основные этапы сборки
1. **Сборка MkDocs** (`mkdocs build`)  
   Генерация сайта с использованием кастомной темы (`theme/`).  

2. **Проверка HTML** (`npm run lint:html`)  
   Валидация с помощью `htmlhint`.  

3. **Минификация HTML** (`npm run minify:html`)  
   Сжатие итоговых страниц для ускорения загрузки.  

4. **Обработка CSS через PostCSS** (`npm run build:css`)  
   Автоматическое добавление вендорных префиксов.  

5. **Деплой на GitHub Pages** (`mkdocs gh-deploy --force`)  

## 🖼️ Кастомная тема
- `theme/base.html` – базовый шаблон (meta, header, footer, js/css)  
- `theme/main.html` – блок контента  
- `theme/partials/header.html` и `footer.html` – хедер и футер  

## 🌍 Деплой
Сайт автоматически публикуется в ветку `gh-pages` и доступен по адресу:  
👉 [https://mento1os.github.io/python-actions-mkdons/](https://mento1os.github.io/python-actions-mkdons/)

## 👨‍💻 Автор
mento1os

