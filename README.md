# 📚 Tugas Laravel Selama PKL (Prakerin)

Repositori tugas mata pelajaran **Pemrograman Web (Laravel)** untuk siswa **Kelas XI PPLG** (Pengembangan Perangkat Lunak dan Gim) yang sedang melaksanakan **PKL / Prakerin**.

Tujuan: siswa tetap belajar dan terukur perkembangannya selama PKL, dengan tugas yang bisa dikerjakan mandiri di sela-sela kegiatan di tempat PKL.

---

## 🎯 Capaian Pembelajaran
Setelah menyelesaikan seluruh tugas, siswa mampu:
1. Menginstal dan mengonfigurasi proyek Laravel.
2. Membuat route, controller, dan view dengan Blade.
3. Mengelola database memakai migration, model, dan Eloquent.
4. Membuat aplikasi CRUD lengkap dengan validasi.
5. Membuat relasi antar tabel (one-to-many, many-to-many).
6. Membuat sistem autentikasi dan hak akses (role).
7. Mengunggah file dan membuat REST API sederhana.
8. Memakai Git & GitHub untuk mengelola dan mengumpulkan pekerjaan.

## 🧰 Persiapan
- PHP >= 8.2, Composer, Node.js & npm
- MySQL / MariaDB (XAMPP / Laragon)
- Git & akun GitHub
- Code editor (VS Code) dan Postman (untuk tugas API)

## 🗓️ Jadwal Tugas (12 Minggu)

| Minggu | Tugas | Topik | Bobot |
|:--:|--|--|:--:|
| 1 | [Tugas 01](tugas/01-setup-dan-routing.md) | Instalasi, struktur folder, routing | 5% |
| 2 | [Tugas 02](tugas/02-blade-templating.md) | Blade, layout, komponen | 5% |
| 3 | [Tugas 03](tugas/03-migration-model-seeder.md) | Migration, Model, Seeder, Factory | 8% |
| 4 | [Tugas 04](tugas/04-crud-dasar.md) | CRUD dasar | 10% |
| 5 | [Tugas 05](tugas/05-validasi-form.md) | Validasi & Form Request | 7% |
| 6 | [Tugas 06](tugas/06-relasi-eloquent.md) | Relasi Eloquent | 10% |
| 7 | [Tugas 07](tugas/07-autentikasi.md) | Autentikasi (login, register, logout) | 8% |
| 8 | [Tugas 08](tugas/08-middleware-role.md) | Middleware & hak akses (role) | 7% |
| 9 | [Tugas 09](tugas/09-upload-file.md) | Upload file, pagination, search | 7% |
| 10 | [Tugas 10](tugas/10-rest-api.md) | REST API + Postman | 8% |
| 11–12 | [Proyek Akhir](tugas/11-proyek-akhir.md) | Mini aplikasi sesuai kasus di tempat PKL | 25% |

> Tambahan: **Jurnal mingguan** ([template](jurnal/TEMPLATE-jurnal-mingguan.md)) tidak masuk bobot di atas, tetapi menjadi syarat kelengkapan nilai.

## 📤 Cara Mengumpulkan Tugas

1. **Fork** repositori ini ke akun GitHub kamu.
2. Buat proyek Laravel di **repositori terpisah** milikmu, misal `laravel-pkl-NAMAKAMU`. Satu repo untuk semua tugas, **commit per tugas** (lihat aturan commit di bawah).
3. Di fork-mu, buat file: `pengumpulan/KELAS-NAMA/tugas-XX.md` (contoh: `pengumpulan/XI-PPLG-1-budi/tugas-01.md`) berisi:
   - Link repo proyek / link commit
   - Screenshot hasil (minimal 2)
   - Catatan kendala (opsional)
4. Buka **Pull Request** ke repositori ini dengan judul: `[Tugas XX] Nama - Kelas`.
5. Guru akan memberi review dan nilai lewat komentar PR.

### Aturan Commit
Gunakan pesan commit yang jelas, contoh:
```
tugas-03: tambah migration tabel produk
tugas-04: buat CRUD produk
```

### Aturan Umum
- Tugas dikerjakan **individu** (kecuali proyek akhir bila ditentukan lain).
- Dilarang menyalin kode teman. Boleh membaca dokumentasi dan bertanya, tapi tulis dan pahami kodenya sendiri.
- Terlambat mengumpulkan: nilai dikurangi 10% per minggu keterlambatan.
- Pastikan `.env` **tidak** ikut ter-commit (gunakan `.env.example`).
- Sertakan `README.md` di repo proyekmu berisi cara instalasi.

## 📊 Penilaian
Lihat [rubrik penilaian](RUBRIK-PENILAIAN.md).

## 🔗 Referensi
- [Dokumentasi Laravel](https://laravel.com/docs)
- [Laracasts - Laravel From Scratch](https://laracasts.com)
- [Tailwind CSS](https://tailwindcss.com) / [Bootstrap](https://getbootstrap.com)
- [Pro Git (Bahasa Indonesia)](https://git-scm.com/book/id/v2)
