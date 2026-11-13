# EduKids LMS

Sistem pengelolaan akademik bimbingan belajar siswa SD untuk program Matematika dan Bahasa Inggris: absensi per sesi, nilai per aspek kompetensi, dan kenaikan level.

## Language

### Orang

**Admin**:
Pengguna yang mengelola data master (siswa, kelas, aspek, aturan level) dan satu-satunya yang boleh mengoreksi data yang sudah dikunci.
_Avoid_: Administrator sistem, superuser

**Tutor**:
Pengajar yang menginput absensi dan nilai untuk kelas yang diampunya.
_Avoid_: Guru, pengajar

**Orang Tua**:
Pengguna dengan akses hanya-baca untuk memantau perkembangan anaknya.
_Avoid_: Wali

**Siswa**:
Anak SD yang mengikuti bimbingan. Tidak memiliki akun login.
_Avoid_: Murid, anak didik

### Akademik

**Mata Pelajaran**:
Salah satu dari dua program: Matematika atau Bahasa Inggris.
_Avoid_: Program, subjek

**Kelas**:
Kelompok siswa yang dibimbing seorang tutor untuk satu Mata Pelajaran.
_Avoid_: Rombel, grup

**Sesi**:
Satu pertemuan satu Kelas pada satu tanggal dan jam untuk satu Mata Pelajaran. Kehadiran dicatat per Sesi, jadi siswa yang ikut dua Mata Pelajaran punya kehadiran terpisah.
_Avoid_: Pertemuan, jadwal

**Absensi**:
Catatan kehadiran seorang Siswa pada satu Sesi.
_Avoid_: Presensi, kehadiran

**Aspek Kompetensi**:
Dimensi penilaian yang khusus untuk satu Mata Pelajaran dan dikelola Admin.
_Avoid_: Komponen nilai, kriteria

**Nilai**:
Angka 0 sampai 100 untuk seorang Siswa pada satu Aspek Kompetensi.
_Avoid_: Skor

### Level

**Level**:
Tingkat penguasaan seorang Siswa pada satu Mata Pelajaran. Setiap Siswa punya satu Level per Mata Pelajaran.
_Avoid_: Tingkat, grade

**Level Gabungan**:
Tampilan turunan yang dihitung dari Level Matematika dan Level Bahasa Inggris seorang Siswa. Bukan data yang diinput.
_Avoid_: Level total, level rata-rata

**Rekomendasi Kenaikan**:
Usulan sistem agar seorang Siswa naik Level, berdasarkan ambang batas yang diatur Admin. Belum berlaku sampai disetujui manusia.
_Avoid_: Kenaikan otomatis

**Periode Penilaian**:
Rentang N Sesi terakhir (diatur Admin) yang dipakai untuk menghitung Rekomendasi Kenaikan.
_Avoid_: Semester, termin

**Sesi Terkunci**:
Sesi yang Absensi dan Nilainya tidak bisa lagi diubah Tutor, hanya dikoreksi Admin.
_Avoid_: Final, tertutup

**Koreksi**:
Perubahan Admin atas data Sesi Terkunci, dicatat beserta pelaku, waktu, nilai lama dan baru.
_Avoid_: Edit, revisi

**Persetujuan Kenaikan**:
Keputusan Admin atau Tutor yang menjadikan Rekomendasi Kenaikan berlaku.
_Avoid_: Konfirmasi
