# Deploy NH Parfum Store v13 ke Netlify

Project ini static dan siap Netlify.

## File penting

- `index.html` — halaman customer.
- `admin/index.html` — halaman Decap CMS admin.
- `admin/config.yml` — struktur field admin.
- `data/settings.json` — profil, hero, banner, section.
- `data/products.json` — daftar produk, gambar, variasi, harga.
- `assets/uploads/` — folder upload gambar dari admin.

## Build settings Netlify

- Branch: `main`
- Base directory: kosong
- Build command: kosong
- Publish directory: `.`

## Wajib untuk admin online

Aktifkan di Netlify:

1. Identity
2. Registration: Invite only
3. Services → Git Gateway → Enable
4. Invite email admin

Admin login lewat:

`https://nama-site.netlify.app/admin/`
