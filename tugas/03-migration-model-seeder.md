# Tugas 03 – Migration, Model, Seeder & Factory
**Minggu:** 3 | **Bobot:** 8% | **Level:** ⭐⭐

## Tujuan
Mengelola struktur database dengan migration dan mengisi data dummy.

## Studi Kasus
Aplikasi **Inventaris Barang** (atau kasus lain yang relevan dengan tempat PKL — konsultasikan ke guru).

## Instruksi
1. Konfigurasi database MySQL di `.env`.
2. Buat migration + model: `php artisan make:model Kategori -m` dan `Barang -m`.
3. Struktur tabel:
   - **kategori**: `id`, `nama`, `timestamps`
   - **barang**: `id`, `kategori_id` (FK), `kode` (unique), `nama`, `stok` (int), `harga` (decimal), `deskripsi` (nullable), `timestamps`
4. Buat **Seeder** untuk kategori (min. 5 data) dan **Factory** untuk barang (min. 30 data, pakai Faker).
5. Jalankan `php artisan migrate:fresh --seed`.
6. Buat route `/barang` yang menampilkan semua data barang dalam tabel (pakai Eloquent `Barang::all()`).
7. Coba di `php artisan tinker`: `create`, `find`, `where`, `update`, `delete`. **Tulis hasil percobaanmu** di file `catatan-tinker.md`.

## Output yang Dikumpulkan
- Link repo
- Screenshot struktur tabel di phpMyAdmin/DBeaver
- Screenshot halaman `/barang`
- File `catatan-tinker.md`

## Tantangan Bonus ⭐⭐
Tambahkan `softDeletes` pada tabel barang.
