# Just Dialog — Лендинг сайт

SEO-оптимизированный одностраничный сайт для сервиса Just Dialog.

## Структура проекта

```
drawbridge-dialog/
├── index.html          # Главная HTML страница
├── styles.css          # Стили CSS
├── script.js           # JavaScript функциональность
├── hero-dashboard.svg  # Главное изображение dashboard
├── icon-*.svg          # Иконки для функций
└── README.md           # Этот файл
```

## Возможности

### SEO оптимизация
- ✅ Семантическая HTML5 разметка
- ✅ Один H1, правильная иерархия H2/H3
- ✅ Schema.org разметка (Organization, FAQPage, BreadcrumbList)
- ✅ Meta теги для SEO и Open Graph
- ✅ ALT теги для всех изображений
- ✅ Внутренняя перелинковка (anchor-ссылки)
- ✅ Ключевые слова естественно интегрированы

### Ключевые слова
- WhatsApp CRM
- Telegram CRM
- единое окно переписок
- управление чатами
- обработка заявок из мессенджеров
- чат для бизнеса Казахстан
- WhatsApp для продаж

### Дизайн
- Минималистичный, современный стиль
- Цветовая схема: серый, белый, голубой акцент
- Адаптивный дизайн (mobile-first)
- Быстрая загрузка (SVG иконки)
- Без анимаций перегруза

### Функциональность
- Интерактивное FAQ с раскрытием ответов
- Форма обратной связи
- Плавная прокрутка к якорям
- Подсветка активного раздела в навигации

## Запуск проекта

### Локально
Откройте файл `index.html` в браузере:
```bash
open index.html
```

### С локальным сервером
```bash
# Python 3
python -m http.server 8000

# или Python 2
python -m SimpleHTTPServer 8000
```

Откройте http://localhost:8000 в браузере.

## Настройка

### Контактная информация
Замените в файле `index.html`:
- Телефоны: `+7 (7XX) XXX-XX-XX` → ваш номер
- WhatsApp: `77XXXXXXXXX` → ваш номер
- Telegram: `justdialog_support` → ваш username
- Email: `info@justdialog.kz` → ваш email
- URL: `https://justdialog.kz` → ваш домен

### Изображения
Замените SVG файлы на реальные скриншоты продукта:
- `hero-dashboard.svg` - главное изображение интерфейса
- `icon-*.svg` - иконки для функций (или оставьте SVG)

### Форма обратной связи
В файле `script.js` настройте отправку формы на ваш сервер:
```javascript
// Строка 28-30
// Замените console.log на fetch запрос к вашему API
fetch('/api/contact', {
    method: 'POST',
    body: JSON.stringify(data)
})
```

## Производительность

### Оптимизация
- SVG иконки вместо растровых изображений
- Минимальные зависимости (только Google Fonts)
- Ленивая загрузка изображений (`loading="lazy"`)
- Критичные стили inline (можно добавить)

### Дальнейшая оптимизация
```bash
# Минификация CSS
npx clean-css-cli styles.css -o styles.min.css

# Минификация JS
npx terser script.js -o script.min.js

# Минификация HTML
npx html-minifier index.html -o index.min.html
```

## Проверка SEO

### Инструменты
- [Google PageSpeed Insights](https://pagespeed.web.dev/)
- [Google Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)
- [Schema Markup Validator](https://validator.schema.org/)
- [Google Rich Results Test](https://search.google.com/test/rich-results)

### Чек-лист перед публикацией
- [ ] Замените placeholder контакты на реальные
- [ ] Добавьте реальные изображения/скриншоты
- [ ] Настройте форму обратной связи
- [ ] Проверьте Schema разметку
- [ ] Протестируйте на мобильных устройствах
- [ ] Настройте SSL сертификат (HTTPS)
- [ ] Создайте sitemap.xml
- [ ] Создайте robots.txt
- [ ] Добавьте Google Analytics / Яндекс.Метрику
- [ ] Настройте Open Graph изображения

## Deployment

### GitHub Pages
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repo.git
git push -u origin main
```
Включите GitHub Pages в настройках репозитория.

### Netlify / Vercel
Перетащите папку проекта в интерфейс или подключите GitHub репозиторий.

## Лицензия

Все права защищены © 2025 Just Dialog

## Поддержка

Для вопросов: info@justdialog.kz