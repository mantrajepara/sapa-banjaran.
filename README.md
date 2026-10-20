# SAPA BANJARAN — Versi Awal

Website statis responsif tanpa build step. Berkas: `index.html`, `style.css`, `app.js`, `manifest.webmanifest`.

## Jalankan lokal
Buka `index.html` di browser, atau gunakan server lokal:

```bash
python -m http.server 8000
```

Kemudian buka http://localhost:8000.

## Deploy ke Wasmer
1. Buat repository GitHub, lalu unggah keempat file aplikasi (bukan ZIP) ke root repository.
2. Masuk ke dashboard Wasmer di https://wasmer.io/ dan cari opsi pembuatan/deployment aplikasi dari GitHub atau static site sesuai opsi yang tersedia pada akun Anda.
3. Pilih repository, gunakan root sebagai direktori publik. Tidak diperlukan perintah build untuk aplikasi statis ini.
4. Jalankan deployment dan buka URL `*.wasmer.app` yang diberikan platform.
5. Jika dashboard mengharuskan konfigurasi runtime/server khusus, ikuti dokumentasi Wasmer terkini untuk hosting static website. Alternatif mudah untuk file statis: GitHub Pages, Cloudflare Pages, atau Netlify.

## Batasan penting
- Aspirasi disimpan di `localStorage` masing-masing browser, **bukan** server; warga lain dan pengelola tidak dapat melihatnya.
- Dashboard admin hanyalah **demo tanpa autentikasi**, jangan gunakan untuk laporan warga sungguhan.
- Jangan meminta NIK, nomor telepon, alamat lengkap, atau data sensitif pada prototipe.
- Untuk produksi, tambahkan backend/database, login admin, pengaturan akses, validasi, perlindungan spam, kebijakan privasi, dan persetujuan pemrosesan data.
- Berita dan agenda saat ini adalah konten contoh.
