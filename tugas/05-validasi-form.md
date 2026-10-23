# Tugas 05 – Validasi & Form Request
**Minggu:** 5 | **Bobot:** 7% | **Level:** ⭐⭐

## Tujuan
Memvalidasi input pengguna dan menampilkan pesan error yang jelas.

## Instruksi
1. Buat Form Request: `php artisan make:request StoreBarangRequest` dan `UpdateBarangRequest`.
2. Aturan validasi minimal:
   - `kode`: wajib, unik (saat update, abaikan ID sendiri), maks 20 karakter
   - `nama`: wajib, min 3 karakter
   - `stok`: wajib, integer, minimal 0
   - `harga`: wajib, numeric, minimal 100
   - `kategori_id`: wajib, harus ada di tabel kategori (`exists`)
3. Tampilkan pesan error per field dengan `@error` dan pertahankan input lama dengan `old()`.
4. Ubah pesan error ke **Bahasa Indonesia** (lewat method `messages()` atau file bahasa).
5. Terapkan validasi yang sama untuk form **Kategori**.

## Output yang Dikumpulkan
- Link repo
- Screenshot form dengan error untuk tiap aturan (minimal 3)

## Tantangan Bonus ⭐⭐
Buat **custom rule** (`php artisan make:rule`), misal kode barang harus berformat `BRG-0001`.
