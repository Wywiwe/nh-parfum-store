# NH Parfum Store — Netlify Ready v12

Struktur ini sudah dipisah untuk hosting Netlify:

```text
index.html              # website publik
data/store.json         # semua data toko, banner, produk, harga
admin/index.html        # panel admin CMS
admin/config.yml        # konfigurasi Decap CMS
assets/uploads/         # folder gambar upload dari admin
netlify.toml            # konfigurasi deploy Netlify
_redirects              # redirect /admin ke /admin/
```

## Cara deploy yang benar

Untuk website publik biasa, folder ini bisa di-drag ke Netlify Drop.

Tapi agar admin `/admin/` bisa menyimpan perubahan produk/gambar ke semua customer, project harus terhubung ke GitHub/GitLab melalui Netlify, lalu aktifkan Git Gateway/Identity di dashboard Netlify.

Langkah ringkas:

1. Upload folder ini ke repository GitHub.
2. Di Netlify: Add new site → Import from Git → pilih repository.
3. Build command dikosongkan.
4. Publish directory: `.`
5. Deploy.
6. Di Netlify dashboard, aktifkan Identity.
7. Set registration ke Invite only.
8. Aktifkan Git Gateway.
9. Invite email admin.
10. Buka `https://domain-lu.netlify.app/admin/` untuk edit website.

## Ukuran gambar

- Banner ideal: 1600 × 900 px, rasio 16:9.
- Produk ideal: 1080 × 1080 px, rasio 1:1.
- Website memakai `object-fit: contain`, jadi gambar tampil utuh dan tidak dipotong.

## Catatan penting

- Admin sekarang bukan password di HTML lagi.
- Data tidak pakai localStorage lagi untuk produk/banner/profil.
- Produk, banner, profil, harga, dan gambar tersimpan ke file `data/store.json` dan `assets/uploads/` melalui CMS.
- Cart dan nama customer tetap disimpan lokal di perangkat customer karena itu memang data pribadi/perangkat.
