# Tugas 10 – REST API dengan Laravel
**Minggu:** 10 | **Bobot:** 8% | **Level:** ⭐⭐⭐⭐

## Tujuan
Membuat REST API dan mengujinya dengan Postman.

## Instruksi
1. Siapkan API: `php artisan install:api` (Laravel Sanctum).
2. Buat `Api\BarangController` dan daftarkan route di `routes/api.php`.
3. Endpoint wajib:
   | Method | Endpoint | Keterangan |
   |--|--|--|
   | POST | `/api/login` | Mengembalikan token |
   | POST | `/api/logout` | Hapus token (butuh auth) |
   | GET | `/api/barang` | Daftar barang (paginate) |
   | GET | `/api/barang/{id}` | Detail barang |
   | POST | `/api/barang` | Tambah barang (butuh auth) |
   | PUT | `/api/barang/{id}` | Ubah barang (butuh auth) |
   | DELETE | `/api/barang/{id}` | Hapus barang (butuh auth) |
4. Gunakan **API Resource** (`php artisan make:resource BarangResource`) untuk format JSON.
5. Format respon konsisten:
   ```json
   { "success": true, "message": "...", "data": { } }
   ```
6. Gunakan status HTTP yang tepat (200, 201, 401, 404, 422).
7. Buat **Postman Collection** dan export ke `docs/postman_collection.json`.

## Output yang Dikumpulkan
- Link repo
- File `docs/postman_collection.json`
- Screenshot hasil request di Postman (sukses & gagal)
- Dokumentasi endpoint singkat di README

## Tantangan Bonus ⭐⭐⭐⭐
Buat halaman frontend sederhana (HTML + `fetch`) yang mengonsumsi API tersebut.
