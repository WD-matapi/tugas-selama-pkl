# Panduan Guru: Pengaturan Absensi & Interaksi

## A. Pengaturan Awal (sekali saja)
1. **Settings → General → Features**: pastikan **Issues** dan **Discussions** aktif.
2. **Settings → Actions → General → Workflow permissions**: pilih **Read and write permissions**, lalu Save.
3. Buka tab **Actions** → **Setup Labels** → **Run workflow** (membuat label `absensi`, `terverifikasi`, `ditolak`, `tanya-guru`, `terjawab`).
4. Edit `absensi/daftar-siswa.csv`: ganti contoh dengan data siswa (nama, kelas, **username GitHub**, tempat PKL).
5. Undang siswa sebagai **collaborator** (opsional). Siswa tetap bisa membuat Issue di repo publik tanpa itu.
6. Jika username guru bukan `aktivitasRudi`, ganti nilai `assignees` pada file di `.github/ISSUE_TEMPLATE/`.

## B. Rutinitas Mingguan
1. Buka **Issues** → filter `label:absensi -label:terverifikasi -label:ditolak`.
2. Cek link bukti. Jika valid → tambahkan label **terverifikasi**. Jika tidak → label **ditolak** + komentar alasan.
3. Rekap `REKAP-ABSENSI.md` ter-update otomatis setiap ada perubahan label (atau jalankan manual: Actions → Rekap Absensi → Run workflow).
4. Cek siswa yang masih "–" (belum absen) dan tegur lewat WhatsApp / komentar.

## C. Menjawab Pertanyaan Siswa
- Filter `label:tanya-guru is:open`. Balas di komentar, lalu tambahkan label **terjawab** dan tutup Issue.

## D. Review Tugas
- Beri umpan balik di Pull Request siswa memakai fitur **Review** (Approve / Request changes) dan tulis nilai di komentar.

## E. Menghitung Nilai Keaktifan (10% nilai akhir)
| Komponen | Bobot | Sumber data |
|--|:--:|--|
| Kehadiran mingguan (absensi terverifikasi) | 50% | `REKAP-ABSENSI.md` (kolom %) |
| Bertanya / menjawab di Issue & Discussions | 20% | label `tanya-guru` & komentar |
| Peer review PR teman (min. 4) | 20% | komentar review di PR |
| Hadir sesi konsultasi online | 10% | catatan guru |

## F. Catatan Penting
- Workflow `Rekap Absensi` memerlukan file `absensi/daftar-siswa.csv` dengan format kolom persis: `nama,kelas,github_username,tempat_pkl` (tanpa koma di dalam isian).
- Jika repo **private**, siswa harus dijadikan collaborator agar bisa membuka Issue.
