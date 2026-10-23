# Tugas 01 – Instalasi, Struktur Folder & Routing
**Minggu:** 1 | **Bobot:** 5% | **Level:** ⭐

## Tujuan
Mampu menginstal Laravel, memahami struktur folder, dan membuat route dasar.

## Materi Singkat
- `composer create-project laravel/laravel nama-proyek`
- Struktur folder: `app/`, `routes/`, `resources/views/`, `database/`, `public/`
- File `routes/web.php`, `.env`, `php artisan serve`

## Instruksi
1. Buat proyek Laravel baru bernama `laravel-pkl-NAMAKAMU`.
2. Inisialisasi Git, buat repo di GitHub, lalu push (pastikan `.env` tidak ikut).
3. Buat route berikut di `routes/web.php`:
   | URL | Output |
   |--|--|
   | `/` | Halaman selamat datang berisi nama & kelas |
   | `/profil` | Profil singkat (nama, sekolah, tempat PKL) |
   | `/tentang-pkl` | Deskripsi kegiatan PKL kamu |
   | `/hitung/{a}/{b}` | Menampilkan hasil penjumlahan, pengurangan, perkalian a dan b |
   | `/salam/{nama?}` | Menampilkan "Halo, {nama}" (default: "Tamu") |
4. Beri nama pada setiap route (`->name('profil')`).
5. Tambahkan route fallback untuk halaman 404 kustom.

## Output yang Dikumpulkan
- Link repo GitHub
- Screenshot semua route di browser
- Hasil `php artisan route:list`

## Tantangan Bonus ⭐
Batasi parameter `{a}` dan `{b}` hanya angka dengan `->where()`.
