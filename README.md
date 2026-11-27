# TruckStop

Магазин аксессуаров и товаров для грузовых автомобилей.
**Локация:** окружная Тбилиси (продажа с машины + онлайн).

Сайт: https://alexberik.github.io/truckstop/

## Структура репозитория

```
index.html                       — сайт (статический HTML, каталог виден поисковикам и ИИ)
tailwind.css                     — стили (собраны локально, без CDN)
truckstop-images/brand/          — логотип, баннеры
truckstop-images/products/       — фото товаров (jpg + webp)
google0afb946164473d6a.html      — подтверждение Google Search Console (не удалять, держать в корне)
robots.txt, sitemap.xml          — для поисковиков
.nojekyll                        — отключает Jekyll на GitHub Pages
```

## Публикация (GitHub Pages)

Settings → Pages → Source: Deploy from a branch → Branch: `main`, папка `/ (root)` → Save.

## Что осталось заполнить

В `index.html` найди и замени:

- `https://wa.me/995` (2 места) → `https://wa.me/ТВОЙ_НОМЕР` (в международном формате, без + и пробелов)
- `href="#"` у иконок Instagram, Facebook, TikTok → ссылки на твои страницы
- Строка «Ссылки скоро будут активны» → удалить, когда ссылки вставлены

## Добавить товар

Скопируй блок `<article class="product-cell" ...>` в разделе каталога, поменяй имя файла фото, артикул, название и `data-cat` (`kitchen`, `holders`, `light`, `comfort`, `supplies`).
Фото кладутся в `truckstop-images/products/` в двух форматах: `имя.jpg` и `имя.webp`.
