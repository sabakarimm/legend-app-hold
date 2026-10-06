# Legend App Holding Page (app.legendmemory.ai)

Static single-page site matching legendmemory.ai branding. No build step.

## App Store switch

In `index.html`:

```js
const APP_STORE_URL = "";
```

Empty = holding page. Set to App Store URL = redirect (`location.replace` + meta refresh).

## Assets

- `assets/logo.png` - Legend wordmark + icon (from Shopify CDN)
- `assets/icon.png` - Legend icon mark

## Local preview

```bash
cd site && python3 -m http.server 8766
```

## Deploy

Publish `site/` only. Point Namecheap **CNAME host `app`** at your static host. Do not change apex Shopify DNS for legendmemory.ai.
