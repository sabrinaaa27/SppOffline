# SIM SPP — Sistem Informasi Manajemen SPP & Pembayaran Sekolah

Aplikasi offline tanpa server untuk tugas Sistem Informasi Manajemen SPP.

## Login
Username: `sabrina`
Password: `juraini`

Password diverifikasi menggunakan SHA-256. Hash juga tersedia di `data/admin.json`.

## Fitur utama
- Login admin offline.
- Dashboard periode bulanan dengan total tagihan, penerimaan, saldo tunggakan, dan status lunas.
- Data siswa: tambah, edit, nonaktif, hapus, dan histori pembayaran per siswa.
- Master tarif SPP berdasarkan kelas.
- Generate tagihan SPP otomatis untuk siswa aktif berdasarkan tarif kelas.
- Tagihan individu jika hanya ingin menagihkan siswa tertentu.
- Pembayaran penuh maupun sebagian; nominal dibatasi agar tidak melebihi sisa tagihan.
- Metode pembayaran: Tunai, Transfer, QRIS.
- Histori seluruh transaksi.
- Bukti pembayaran siap cetak.
- Laporan tunggakan siswa per periode.
- Rekap tagihan/pembayaran dan cetak laporan.
- Export/Import database JSON.
- Database transaksi memakai IndexedDB pada browser.

## Cara menjalankan
Ekstrak ZIP lalu buka `index.html` pada browser modern.

Tidak membutuhkan PHP, MySQL, Node.js, XAMPP, atau server.

## Catatan database
Karena offline tanpa server, IndexedDB menjadi database lokal pada browser/perangkat yang digunakan. Backup berkala menggunakan menu Export JSON agar data tidak hilang saat browser dibersihkan.
