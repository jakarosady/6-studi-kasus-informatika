# Studi Kasus 4 — Klasifikasi Risiko Keterlambatan Layanan

![ML](https://img.shields.io/badge/Topik-Machine%20Learning-blueviolet) ![Evaluasi](https://img.shields.io/badge/Evaluasi-train%2Ftest-blue)

## Ringkasan
Materi keempat membahas konsep AI, machine learning, deep learning, workflow data, supervised dan unsupervised learning, klasifikasi/regresi, pembagian training/testing, evaluasi, deployment, kualitas data, bias, keamanan, dan keterbatasan model. Proyek ini menggunakan **supervised classification** untuk memprediksi risiko keterlambatan layanan dari data sintetis.

## Rumusan masalah
Dapatkah model mempelajari pola sederhana dari fitur operasional untuk mengidentifikasi pesanan yang berisiko terlambat? Notebook memuat pembuatan data, pemisahan train/test, preprocessing, pelatihan model, dan evaluasi.

## Batasan masalah
- Data sintetis; hubungan fitur dengan label sengaja dibuat untuk pembelajaran.
- Model tidak boleh dipakai untuk keputusan nyata tanpa data representatif, validasi, pemantauan, dan persetujuan pihak terkait.
- Hasil pada data uji hanya mengukur performa pada sampel simulasi ini.
- Fitur/label simulasi dapat mengandung pola yang tidak ditemukan di dunia nyata.
- Tidak ada klaim kausalitas dan tidak ada jaminan performa di luar distribusi data pelatihan.

## Tujuan pembelajaran
- Menjalankan workflow machine learning yang dapat direproduksi.
- Menghindari kebocoran data dengan pipeline preprocessing.
- Membaca confusion matrix, precision, recall, F1, dan accuracy.
- Menjelaskan keterbatasan kualitas data dan generalisasi.

## Metodologi
1. Buat dataset sintetis dengan seed tetap.
2. Pisahkan data latih dan uji secara stratified.
3. Gunakan `Pipeline` untuk preprocessing dan klasifikasi.
4. Evaluasi pada data uji yang tidak digunakan saat pelatihan.
5. Tinjau fitur penting secara hati-hati dan diskusikan bias serta monitoring.

## Menjalankan
```bash
pip install -r ../requirements.txt
jupyter lab
```
Buka `studi_kasus_04_machine_learning.ipynb`, kemudian pilih **Run All**.

