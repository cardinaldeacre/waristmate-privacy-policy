# WaristMate — Halaman Kebijakan Privasi

Halaman kebijakan privasi statis satu halaman untuk **WaristMate**, aplikasi pengelolaan dan perhitungan warisan Islami (Faraidh).

## Gambaran Umum

Repositori ini berisi satu file `index.html` mandiri dengan konten Kebijakan Privasi lengkap, didesain sesuai identitas WaristMate (palet warna hijau tua dan emas dengan motif bintang khas Islami). Halaman ini mencakup:

- Daftar isi (table of contents) yang sticky di sisi kiri (desktop) / menu daftar isi yang bisa dibuka-tutup (mobile)
- Scrollspy yang otomatis menyorot bagian yang sedang dibaca
- Tata letak yang sepenuhnya responsif, hingga ke layar mobile kecil
- Tanpa proses build, tanpa dependensi selain Google Fonts (Fraunces, Inter, JetBrains Mono)

## Struktur File

```
.
└── index.html   # Halaman kebijakan privasi lengkap (HTML + CSS + JS, tanpa dependensi eksternal selain font)
```

## Cara Menggunakan

### Melihat secara lokal
Cukup buka `index.html` di browser mana pun — tidak perlu server atau proses build.

### Deploy
Unggah `index.html` ke hosting statis mana pun, misalnya:

- **GitHub Pages** — push repositori ini, aktifkan Pages di pengaturan repo, lalu arahkan ke root atau branch `main`.
- **Netlify / Vercel** — drag and drop folder ini, atau hubungkan repositori untuk auto-deploy.
- **Hosting di dalam aplikasi** — sertakan `index.html` langsung di dalam aplikasi WaristMate dan tautkan dari menu Pengaturan → Kebijakan Privasi.

Setelah di-deploy, gunakan URL tersebut di mana pun tautan Kebijakan Privasi dibutuhkan (misalnya di listing Google Play Store, App Store, atau layar persetujuan Google Sign-In).

## Memperbarui Konten

Seluruh teks kebijakan berada langsung di dalam `index.html`, di dalam blok bernomor `<section class="clause" id="s1">` … `<section class="clause" id="s11">`. Untuk memperbarui:

1. Ubah teks pada bagian yang relevan.
2. Perbarui tanggal `Terakhir diperbarui` pada bagian header (`<span class="updated">`).
3. Daftar isi dan scrollspy dibuat secara otomatis dari bagian-bagian yang ada — tidak perlu diedit manual jika hanya mengubah teks. Jika Anda menambah atau menghapus satu bagian penuh, pastikan penomoran `id="sN"` dan `<span class="clause-num">` tetap konsisten.

## Lisensi

Halaman ini disediakan untuk digunakan oleh WaristMate. Silakan sesuaikan sesuai kebutuhan deployment Anda.
