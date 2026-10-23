# Tugas 04 – CRUD Dasar
**Minggu:** 4 | **Bobot:** 10% | **Level:** ⭐⭐

## Tujuan
Membuat fitur Create, Read, Update, Delete dengan Resource Controller.

## Instruksi
Lanjutkan proyek Tugas 03 (tabel `barang`).
1. Buat resource controller: `php artisan make:controller BarangController --resource --model=Barang`.
2. Daftarkan `Route::resource('barang', BarangController::class)`.
3. Buat view: `index`, `create`, `edit`, `show`.
4. Fitur wajib:
   - Tampilkan daftar barang beserta nama kategorinya
   - Tambah, ubah, hapus barang
   - Konfirmasi sebelum hapus (JavaScript `confirm` atau modal)
   - Pesan sukses/gagal memakai `session('success')` (flash message)
5. Gunakan `@csrf` dan `@method('PUT')` / `@method('DELETE')` dengan benar.
6. Dropdown kategori pada form diambil dari database.
7. Buat juga CRUD untuk **Kategori**.

## Output yang Dikumpulkan
- Link repo
- Video singkat (≤ 2 menit) / GIF demo CRUD, atau 5 screenshot (index, create, edit, show, hapus)

## Tantangan Bonus ⭐⭐
Tambahkan fitur "stok menipis" (badge merah bila stok < 5).
