# Tugas 07 – Autentikasi
**Minggu:** 7 | **Bobot:** 8% | **Level:** ⭐⭐⭐

## Tujuan
Membuat sistem login, registrasi, dan logout.

## Instruksi
1. Pilih salah satu pendekatan:
   - **(Disarankan untuk belajar)** Buat manual dengan `Auth::attempt()`, `Auth::logout()`, `Hash::make()`.
   - Atau pakai **Laravel Breeze** (jelaskan file apa saja yang dihasilkan).
2. Fitur wajib: register, login, logout, halaman dashboard (hanya untuk user login).
3. Lindungi semua route CRUD dengan middleware `auth`.
4. Tampilkan nama user yang login di navbar.
5. Validasi: email unik, password min 8 karakter + konfirmasi password.
6. Tambahkan fitur **ubah password** di halaman profil.
7. Jangan menyimpan password sebagai plain text!

## Output yang Dikumpulkan
- Link repo
- Screenshot: register, login gagal, login sukses, dashboard, akses halaman terproteksi tanpa login (redirect)
- Jawab: apa perbedaan *hashing* dan *enkripsi*? (2–3 kalimat)

## Tantangan Bonus ⭐⭐⭐
Tambahkan fitur "Remember me" dan batasi percobaan login (throttle).
