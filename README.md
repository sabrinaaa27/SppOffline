# SIM SPP — Sistem Informasi Manajemen SPP & Pembayaran Sekolah

Aplikasi web **offline tanpa server** menggunakan HTML, CSS, dan JavaScript. Database utama menggunakan **IndexedDB** pada browser.

## Login demo
- Username: `sabrina`
- Password: `juraini`
- Hash SHA-256 disimpan di `data/admin.json`

## Fitur
- Login admin dengan verifikasi SHA-256 via Web Crypto API.
- Dashboard ringkasan tagihan, pembayaran, tunggakan, dan status pembayaran.
- CRUD data siswa.
- Generate tagihan SPP bulanan.
- Catat pembayaran beserta metode dan histori transaksi.
- Laporan tunggakan.
- Laporan pemasukan bulanan/tahunan.
- Cetak laporan.
- Export/import backup database JSON.

## Menjalankan
Ekstrak ZIP, lalu buka `index.html` di browser modern.

> Catatan teknis: sebagian browser membatasi `fetch()` ke file JSON ketika halaman dibuka langsung melalui `file://`. Agar aplikasi tetap bisa login dalam mode lokal, `app.js` memiliki fallback konfigurasi admin yang identik dengan `data/admin.json`. File JSON tetap disediakan sebagai sumber konfigurasi yang jelas dan dapat dipindahkan/diubah bersama proyek.
