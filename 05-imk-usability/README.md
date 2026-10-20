# Studi Kasus 5 — Audit Usability Portal Layanan Akademik

![IMK](https://img.shields.io/badge/Topik-IMK%20%2F%20UX-orange) ![Aksesibilitas](https://img.shields.io/badge/Fokus-usability%20dan%20aksesibilitas-blue)

## Ringkasan
Dokumen sesi kelima berisi enam modul: Pengantar IMK, Aspek Kognitif & Persepsi, Interaksi Sosial & Konteks Penggunaan, Proses Desain Interaksi & Evaluasi, Analisis Kebutuhan & User Persona, serta Prinsip Visualisasi Data & Dasbor Interaktif. Studi kasus menggabungkan gagasan tersebut dalam audit **portal layanan akademik fiktif**.

## Rumusan masalah
Mahasiswa mengeluhkan proses menemukan jadwal, mengunduh surat, dan memeriksa status permohonan. Tim perlu menentukan tugas yang paling bermasalah, membuat kebutuhan pengguna, serta menyusun perbaikan berdasarkan bukti.

Notebook berisi:
- persona dan kebutuhan fungsional/nonfungsional;
- data pengujian tugas sintetis;
- success rate dan task time;
- simulasi temuan heuristik;
- daftar perbaikan yang ditautkan dengan prinsip IMK dan aksesibilitas;
- visualisasi ringkas tanpa elemen dekoratif berlebihan.

## Batasan masalah
- Seluruh persona, respons, waktu tugas, dan temuan dibuat sebagai contoh sintetis.
- Hasil bukan bukti bahwa portal nyata memiliki masalah yang sama.
- Skor heuristik hanya latihan prioritisasi; evaluasi formal perlu evaluator dan protokol yang sesuai.
- Pemeriksaan angka kontras sederhana tidak sama dengan audit kepatuhan WCAG lengkap.
- Tidak mengumpulkan data pribadi atau data mahasiswa sungguhan.

## Tujuan pembelajaran
- Membedakan kebutuhan fungsional dan nonfungsional.
- Menghubungkan persona, skenario penggunaan, dan rancangan evaluasi.
- Menghitung success rate dan task time.
- Memprioritaskan perbaikan dengan mempertimbangkan feedback, consistency, affordance, cognitive load, aksesibilitas, dan transparansi.

## Metodologi
1. Rumuskan persona serta skenario.
2. Definisikan tugas dan metrik keberhasilan.
3. Analisis data uji kegunaan sintetis.
4. Susun temuan heuristik dan prioritas perbaikan.
5. Rancang prinsip dashboard: overview first, zoom/filter, details-on-demand.

## Menjalankan
```bash
pip install -r ../requirements.txt
jupyter lab
```
Buka `studi_kasus_05_imk_usability.ipynb` dan pilih **Run All**.


