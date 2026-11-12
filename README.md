# TorchFlame

Bağımlılıksız, tek dosyalık HTML5 Canvas meşale/alev oyunu. Çevrimdışı çalışan, telefona yüklenebilir bir PWA'dır.

© 2026 A. Emre Canaslan — MIT Lisansı

## Yapı

```
index.html
manifest.webmanifest
sw.js
_headers
netlify.toml
.nojekyll
LICENSE
README.md
icons/  (icon-192.png, icon-512.png, apple-touch-icon.png)
```

## Kurulum

**GitHub Pages:** Dosyaları reponun köküne gönderin → Settings → Pages → Branch: `main` / `(root)`.

**Cloudflare Pages:** Repoyu bağlayın. Build command: boş bırakın, Output directory: `/` (kök). `_headers` otomatik uygulanır.

**Netlify:** Repoyu bağlayın; `netlify.toml` yapılandırmayı sağlar.

> Not: GitHub Pages `_headers` dosyasını uygulamaz; bu yalnızca Cloudflare/Netlify içindir.

## Telefona yükleme

- **Android (Chrome):** Menü → "Uygulamayı yükle" / "Ana ekrana ekle".
- **iOS (Safari):** Paylaş → "Ana Ekrana Ekle".

## Sürüm güncelleme

`sw.js` içindeki `VERSION` değerini artırıp yayınlayın; eski önbellek otomatik silinir ve uygulama yeni sürüme geçer.

## Yerelde test

```
python3 -m http.server 8080
```

Ardından `http://localhost:8080` adresini açın (service worker için HTTPS veya localhost gerekir).
