# Kasir Sekolah - SD PLUS DARUSSALAM

Ini adalah aplikasi kasir sekolah sederhana yang bisa di-deploy di GitHub Pages.
Fitur:
- Import data pembayaran dari Excel (.xlsx)
- Input & update pembayaran (Admin)
- Cetak kwitansi
- Tampilan publik (read-only)
- Pencarian berdasarkan NISN
- Export rekap ke Excel
- Pengaturan kata sandi admin (disimpan sebagai SHA-256 hash di localStorage)

Cara deploy:
1. Buat repository baru di GitHub (public).
2. Upload semua file dari ZIP ini ke root repo.
3. Settings -> Pages -> branch: main, folder: / (root).
4. Setelah beberapa menit, akses: https://<username>.github.io/<repo>/

Catatan keamanan:
- Aplikasi ini sepenuhnya client-side. Proteksi admin menggunakan hash di localStorage
  yang mudah dimanipulasi jika seseorang menguasai browser. Untuk produksi gunakan backend
  (Firebase, Supabase, dsb) untuk autentikasi dan penyimpanan data.
