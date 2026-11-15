# Home Stock — Lovely Home Organizer

Aplikasi stok kebutuhan rumah tangga berbasis PWA, dibuat dengan HTML, CSS, dan JavaScript tanpa framework.

## Fitur
- Dashboard ringkasan jumlah jenis barang, stok menipis, prioritas belanja, dan estimasi nilai stok.
- Tambah, edit, dan hapus barang.
- Kategori: Dapur, Kamar mandi, Outdoor, Laundry, Kamar tidur, Ruang tamu, Mobil, Sepeda, Beauty.
- Pencarian dan pengurutan stok berdasarkan jumlah, kategori, prioritas, serta harga.
- Catatan transaksi barang masuk, keluar, dan pembelian.
- Data tersimpan di `localStorage` browser.
- Dapat di-cache untuk akses offline setelah kunjungan pertama.

## Cara menjalankan di komputer
Buka folder ini dengan server lokal (jangan hanya membuka `index.html` lewat `file://` agar service worker bisa aktif). Contoh:
```bash
python -m http.server 8000
```
Lalu buka `http://localhost:8000`.

## Deploy ke GitHub Pages
1. Buat repository baru di GitHub.
2. Upload semua file dalam folder ini ke root repository: `index.html`, `manifest.webmanifest`, `sw.js`, dan `icon.svg`.
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
6. Tunggu proses deployment selesai dan buka URL GitHub Pages yang diberikan.

## Instalasi di ponsel
Buka URL GitHub Pages melalui Chrome Android, pilih menu browser, lalu **Install app** atau **Add to Home screen**.

## Catatan penting
- Data aplikasi tersimpan lokal pada browser/perangkat yang digunakan. Data tidak otomatis tersinkron ke perangkat lain atau ke akun GitHub.
- Menghapus data situs/browser dapat menghapus data stok. Lakukan backup berkala sebelum membersihkan data browser.
- Untuk sinkronisasi lintas perangkat, perlu ditambahkan backend/database dan autentikasi.
