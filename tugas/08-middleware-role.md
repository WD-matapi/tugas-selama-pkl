# Tugas 08 – Middleware & Hak Akses (Role)
**Minggu:** 8 | **Bobot:** 7% | **Level:** ⭐⭐⭐

## Tujuan
Membatasi fitur berdasarkan peran pengguna.

## Instruksi
1. Tambahkan kolom `role` pada tabel `users` (`admin`, `petugas`, `viewer`) lewat migration baru.
2. Buat middleware: `php artisan make:middleware CekRole` yang menerima parameter role (contoh: `role:admin,petugas`).
3. Hak akses:
   | Fitur | Admin | Petugas | Viewer |
   |--|:--:|:--:|:--:|
   | Lihat data | ✅ | ✅ | ✅ |
   | Tambah/ubah data | ✅ | ✅ | ❌ |
   | Hapus data | ✅ | ❌ | ❌ |
   | Kelola user | ✅ | ❌ | ❌ |
4. Buat halaman **Kelola User** (khusus admin): daftar user & ubah role.
5. Sembunyikan tombol di tampilan sesuai role (`@can` / `@if(auth()->user()->role === ...)`).
6. Tampilkan halaman **403 Forbidden** kustom.
7. Buat seeder 3 akun (admin, petugas, viewer) dan cantumkan di README.

## Output yang Dikumpulkan
- Link repo
- Screenshot tampilan tiap role + halaman 403
- Tabel akun demo di README repo

## Tantangan Bonus ⭐⭐⭐
Gunakan **Gate / Policy** sebagai pengganti pengecekan manual.
