# EduKids LMS

Aplikasi Learning Management System berbasis web untuk bimbingan belajar siswa SD (Matematika dan Bahasa Inggris): absensi per sesi, nilai per aspek kompetensi, dan kenaikan level.

Status: tahap perencanaan, belum ada kode aplikasi.

## Peran

- **Admin**: mengelola data master, aturan level, dan koreksi data terkunci.
- **Tutor**: menginput absensi dan nilai untuk kelasnya.
- **Orang Tua**: memantau perkembangan anaknya (hanya baca).

## Dokumen

- [Software Request](docs/software-request.md): kebutuhan asli dari sponsor ([PDF](docs/software-request-edukids-lms.pdf)).
- [GLOSSARY.md](GLOSSARY.md): istilah domain yang dipakai di seluruh proyek.
- [Keputusan arsitektur (ADR)](docs/adr): alasan di balik keputusan penting.
- [Issue #1](https://github.com/BintoroCA/edukids/issues/1): spec lengkap. Tiket implementasi (#2 sampai #12) adalah sub-issue-nya dan memiliki urutan ketergantungan.

## Target

- Waktu respon di bawah 2 detik, 50+ pengguna bersamaan, ketersediaan 99%.
- Backup harian ke lokasi terpisah, komunikasi lewat TLS.
- Go-live: 25 Januari 2027 (asumsi, belum dikonfirmasi).
