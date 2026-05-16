# NH Parfum Store v13 - Admin E-commerce Flow

## Alur admin produk

Masuk ke:

`https://nama-site.netlify.app/admin/`

Pilih menu **1. Produk** → **Tambah / Edit / Hapus Produk**.

### Tambah produk baru
1. Klik **Add product** di bagian Daftar Produk.
2. Isi **ID unik / slug**. Contoh: `scndl-v-ice`.
3. Isi nama produk, SKU, kategori, badge, notes aroma, dan deskripsi.
4. Upload gambar produk maksimal 5.
   - Ideal produk: **1080×1080 px**.
   - Rasio: **1:1**.
   - Gambar pertama tampil paling depan.
5. Isi **Variasi & Harga**.
   - Contoh variasi: Standar, Best, Premium.
   - Dalam tiap variasi, isi opsi seperti 15ml, 20ml, 30ml.
   - Harga ditulis angka saja, contoh `35000`.
6. Klik **Save / Publish**.
7. Tunggu Netlify redeploy otomatis sekitar 1–3 menit.

### Edit produk
1. Buka menu **1. Produk**.
2. Klik produk yang mau diedit.
3. Ubah data produk, gambar, variasi, harga, atau stok.
4. Klik **Save / Publish**.

### Hapus produk
1. Buka menu **1. Produk**.
2. Klik produk yang mau dihapus.
3. Klik ikon hapus/tong sampah/remove pada item produk.
4. Klik **Save / Publish**.

### Sembunyikan produk tanpa hapus
Matikan field **Tampilkan produk?**. Produk tidak tampil di website, tapi data masih ada di admin.

## Alur edit tampilan website

Pilih menu **2. Tampilan Website** → **Profil, Banner, Section**.

Yang bisa diedit:
- Nama toko
- Logo inisial
- Tagline
- Nomor WhatsApp
- Hero/banner
- Gambar banner maksimal 5
- Section produk
- Kartu Kenapa NH
- Cara order

## Ukuran gambar rekomendasi

- Gambar produk: **1080×1080 px**, rasio **1:1**.
- Gambar banner: **1600×900 px**, rasio **16:9**.

Website memakai `object-fit: contain`, jadi gambar tampil utuh dan tidak terpotong.
