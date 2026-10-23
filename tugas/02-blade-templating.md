# Tugas 02 – Blade Templating
**Minggu:** 2 | **Bobot:** 5% | **Level:** ⭐

## Tujuan
Membuat tampilan dengan layout Blade yang dapat dipakai ulang.

## Materi Singkat
`@extends`, `@section`, `@yield`, `@include`, `@foreach`, `@if`, komponen Blade (`<x-...>`), Controller.

## Instruksi
1. Buat **layout utama** `resources/views/layouts/app.blade.php` berisi navbar, konten, dan footer.
2. Pasang CSS (Bootstrap atau Tailwind via CDN/Vite).
3. Buat controller `HalamanController` dengan method: `beranda`, `profil`, `kegiatan`, `kontak`.
4. Halaman **kegiatan** menampilkan daftar kegiatan PKL kamu (minimal 5 item, dari **array di controller**) menggunakan `@foreach`.
5. Buat **komponen Blade** `<x-card>` untuk menampilkan tiap kegiatan (judul, tanggal, deskripsi).
6. Pakai `@if / @else` untuk menampilkan pesan "Belum ada kegiatan" bila array kosong.

## Output yang Dikumpulkan
- Link repo (commit `tugas-02`)
- Screenshot 4 halaman

## Tantangan Bonus ⭐⭐
Buat menu navbar yang menandai halaman aktif (`request()->routeIs()`).
