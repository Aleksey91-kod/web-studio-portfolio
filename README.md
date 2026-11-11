# Портфолио веб-студии — демонстрационные проекты

Три демонстрационных сайта для портфолио веб-студии. Чистые HTML/CSS/JS, без сборки и зависимостей — достаточно открыть `index.html`.

> Все проекты демонстрационные: названия компаний, контакты, цены и отзывы вымышлены. Формы работают в демо-режиме и не передают персональные данные.

## Структура

| Папка | Проект | Направление | Что внутри |
|---|---|---|---|
| `/` | Обложка портфолио | — | Страница со ссылками на все три проекта |
| `/remont/` | **ATELIERDOM** | Ремонт квартир | Калькулятор сметы, этапы работ, портфолио объектов, модальная форма |
| `/beauty/` | **ÉLAN STUDIO** | Салон красоты | Фильтр услуг по категориям, мастера, трёхшаговая онлайн-запись |
| `/auto/` | **TORQLAB** | Автосервис | Подбор услуги по симптомам, сетка цен, модальная запись |

## Технически

- Адаптивная вёрстка 375 / 768 / 1024 / 1440, mobile-first breakpoints
- Семантический HTML, `aria`-атрибуты, фокус-кольца, закрытие модалей по `Esc`
- `prefers-reduced-motion`, без горизонтального скрола на мобильных
- SEO: `title`, `description`, Open Graph на каждой странице
- Шрифты Google Fonts с `display=swap`, вся графика — инлайн-SVG (без внешних запросов к изображениям)
- Проверено в Chromium: 0 ошибок консоли, все формы и интерактив рабочие

## Публикация на GitHub Pages

```bash
git init
git add .
git commit -m "Демонстрационное портфолио веб-студии: 3 проекта"
git branch -M main
git remote add origin git@github.com:<USERNAME>/web-studio-portfolio.git
git push -u origin main
```

Затем: **Settings → Pages → Source: Deploy from a branch → main / (root)**.

Сайты будут доступны по адресам:

- `https://<USERNAME>.github.io/web-studio-portfolio/` — обложка портфолио
- `https://<USERNAME>.github.io/web-studio-portfolio/remont/`
- `https://<USERNAME>.github.io/web-studio-portfolio/beauty/`
- `https://<USERNAME>.github.io/web-studio-portfolio/auto/`
