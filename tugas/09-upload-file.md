# Tugas 09 – Upload File, Pagination & Pencarian
**Minggu:** 9 | **Bobot:** 7% | **Level:** ⭐⭐⭐

## Tujuan
Mengelola file unggahan dan menampilkan data dalam jumlah besar secara efisien.

## Instruksi
1. Tambahkan kolom `foto` (nullable) pada tabel `barang`.
2. Form tambah/ubah barang dapat **upload foto** (jpg/png, maks 2 MB). Gunakan validasi `image|mimes|max`.
3. Simpan file memakai `Storage` disk `public`, jalankan `php artisan storage:link`.
4. Tampilkan thumbnail di daftar dan foto besar di detail.
5. Saat barang dihapus atau fotonya diganti, **hapus file lama** dari storage.
6. Tambahkan **pagination** (10 data/halaman) dengan `paginate()` dan `withQueryString()`.
7. Tambahkan **pencarian** (nama/kode) dan **filter kategori**.
8. Tambahkan fitur **sorting** (nama, stok, harga).

## Output yang Dikumpulkan
- Link repo
- Screenshot: form upload, daftar dengan thumbnail, hasil pencarian, pagination

## Tantangan Bonus ⭐⭐⭐
Export daftar barang ke **PDF atau Excel** (misal `barryvdh/laravel-dompdf` atau `maatwebsite/excel`).
