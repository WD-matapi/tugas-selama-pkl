# Tugas 06 – Relasi Eloquent
**Minggu:** 6 | **Bobot:** 10% | **Level:** ⭐⭐⭐

## Tujuan
Memahami dan menerapkan relasi antar tabel.

## Studi Kasus
Kembangkan Inventaris menjadi **Sistem Peminjaman Barang**.

## Struktur Data Tambahan
- **peminjam**: `id`, `nama`, `kelas_atau_unit`, `no_hp`
- **peminjaman**: `id`, `peminjam_id`, `tanggal_pinjam`, `tanggal_kembali`, `status` (`dipinjam`/`kembali`)
- **barang_peminjaman** (pivot): `peminjaman_id`, `barang_id`, `jumlah`

## Instruksi
1. Buat ERD sederhana (gambar/draw.io/dbdiagram.io) dan simpan di `docs/erd.png`.
2. Buat migration & model untuk tabel di atas.
3. Definisikan relasi:
   - `Kategori` **hasMany** `Barang` / `Barang` **belongsTo** `Kategori`
   - `Peminjam` **hasMany** `Peminjaman`
   - `Peminjaman` **belongsToMany** `Barang` (withPivot `jumlah`)
4. Buat form peminjaman: pilih peminjam, pilih beberapa barang + jumlah.
5. Saat disimpan, **kurangi stok** barang; saat dikembalikan, **tambah stok** (gunakan `DB::transaction`).
6. Halaman detail peminjaman menampilkan daftar barang yang dipinjam.
7. Gunakan **eager loading** (`with()`) untuk menghindari masalah N+1.

## Output yang Dikumpulkan
- Link repo
- `docs/erd.png`
- Screenshot form, daftar, dan detail peminjaman
- Penjelasan singkat (3–5 kalimat) apa itu masalah N+1 dan bagaimana kamu mengatasinya

## Tantangan Bonus ⭐⭐⭐
Hitung denda keterlambatan otomatis (misal Rp1.000/hari).
