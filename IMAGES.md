# Truck Stop image assets

All website images are stored in `truckstop-images/`.

- `truckstop-images/brand/` — logo and brand banner
- `truckstop-images/products/` — product photos

Product photos are supplied in JPG and WebP formats. Use WebP in the `<source>` element and JPG as the fallback in each `<picture>` element.

Example:

```html
<picture>
  <source srcset="../truckstop-images/products/19_multivarka.webp" type="image/webp" />
  <img src="../truckstop-images/products/19_multivarka.jpg" alt="24V multicooker for truck cabins" loading="lazy" decoding="async" />
</picture>
```

Use paths relative to the page location: root page uses `truckstop-images/...`; language pages in `ru/` and `ka/` use `../truckstop-images/...`.
