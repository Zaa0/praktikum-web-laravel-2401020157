# Praktikum Pemrograman Web — Pertemuan 9

Proyek Laravel untuk Modul 9 (Pengenalan Laravel dan Pola MVC), dilanjutkan pada Modul 10 dan 11.

## Fitur

- Model `Buku` dengan data contoh (BK001–BK004) tanpa basis data.
- Route `/buku` untuk daftar dan pencarian judul (`?cari=`).
- Route `/buku/{kode}` untuk detail buku; kode tidak ditemukan menghasilkan HTTP 404.
- Dua Blade: `resources/views/buku/index.blade.php` dan `show.blade.php`.

## Menjalankan

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan serve --port=8000
```

Buka http://127.0.0.1:8000/buku

## Struktur Penting

- `app/Models/Buku.php`
- `app/Http/Controllers/BukuController.php`
- `routes/web.php`
- `resources/views/buku/index.blade.php`
- `resources/views/buku/show.blade.php`
- `docs/screenshots/` — bukti pengujian
- `Laporan Praktikum/Laporan PPW 9_2401020157.pdf`
