# Software Request: EduKids LMS

Salinan isi dokumen asli: [software-request-edukids-lms.pdf](./software-request-edukids-lms.pdf). Tanggal: 2026-11-09. Project Sponsor: Akbari.

## Deskripsi

Aplikasi Learning Management System (LMS) berbasis web untuk mengelola kegiatan akademik bimbingan belajar siswa Sekolah Dasar (SD) pada program Matematika dan Bahasa Inggris. Sistem memfasilitasi pencatatan absensi per sesi, pengolahan nilai berbasis aspek kompetensi spesifik tiap mata pelajaran, serta pemantauan kenaikan level (levelling) siswa secara terpisah maupun gabungan dengan cepat dan akurat.

## Business Need

Pertanyaan penilaian (skala 1 Tidak Setuju sampai 4 Sangat Setuju): apakah aplikasi meningkatkan pendapatan, mengurangi biaya operasional, meningkatkan produktivitas pegawai, dan meningkatkan nilai tambah intangible. Jawaban terpilih tidak terbaca dari PDF.

## Business Value

**Intangible:** (a) kepercayaan dan kepuasan orang tua siswa; (b) objektivitas dan standarisasi akademik; (c) kemudahan pengambilan keputusan berbasis data; (d) pengurangan beban kerja administratif.

**Tangible:** (a) efisiensi waktu rekapitulasi data; (b) eliminasi kesalahan input dan kalkulasi; (c) penghematan biaya operasional cetak; (d) peningkatan kapasitas kelola admin dan tutor.

## Nonfunctional Requirements

### Operational
1. Sistem dapat digunakan oleh semua perangkat lunak lainnya. (Ditafsirkan: berjalan di browser modern.)
2. Ketersediaan layanan 99%.
3. Go live sebelum 25 Januari 2018. (Tahun ini tidak masuk akal terhadap tanggal dokumen; diasumsikan 25 Januari 2027, belum dikonfirmasi.)

### Performance
1. Waktu respon tidak lebih dari 2 detik.
2. Mampu diakses lebih dari 50 pengguna bersamaan.
3. Server bersih dari virus.

### Security
1. Akses tanpa otorisasi tidak dimungkinkan.
2. Data hanya dapat diubah oleh administrator sistem. (Lihat [ADR 0004](./adr/0004-tutors-write-attendance-and-grades-with-24h-lock.md) untuk penafsiran.)
3. Seluruh data di-backup setiap 24 jam, hasilnya disimpan di lokasi berbeda dari sistem.
4. Seluruh komunikasi client-server harus aman.

## Catatan

PDF tidak memuat persyaratan fungsional. Persyaratan tersebut dirumuskan lewat sesi tanya jawab dan dicatat di [GLOSSARY.md](../GLOSSARY.md), [docs/adr](./adr), dan issue #1.
