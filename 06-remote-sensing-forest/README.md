# Studi Kasus 6 — Deteksi Awal Perubahan Tutupan Hutan Multi-Sensor

![Remote sensing](https://img.shields.io/badge/Topik-Remote%20Sensing%20%2F%20lingkungan-forestgreen) ![Data](https://img.shields.io/badge/Data-sintetis-lightgrey)

## Ringkasan
Transkrip membahas pemantauan perubahan hutan tropis, peringatan deforestasi, citra optik dan radar, Sentinel-1/Sentinel-2, gangguan awan pada citra optik, serta atribusi *direct drivers*. Pembicara menekankan bahwa citra satelit dapat membantu mengklasifikasikan pola perubahan, tetapi penyebab yang lebih rinci sering memerlukan observasi lapangan.

Notebook ini membangun simulasi **deteksi perubahan multi-sensor** dengan data sintetis untuk menunjukkan bagaimana indikator optik yang tertutup awan dapat dipadukan dengan indikator radar.

## Rumusan masalah
Bagaimana sistem sederhana dapat menandai lokasi yang mungkin mengalami perubahan tutupan hutan ketika sebagian pengamatan optik tidak tersedia akibat awan? Apa perbedaan antara mendeteksi perubahan dan menyatakan penyebabnya?

## Batasan masalah
- Data adalah simulasi sintetis, bukan data Sentinel atau observasi lapangan.
- Ambang perubahan hanya untuk demonstrasi; tidak tervalidasi secara ilmiah.
- Radar dan optik disederhanakan menjadi fitur numerik; tidak memproses citra raster asli.
- Alert bukan konfirmasi deforestasi, legalitas, atau penyebabnya.
- Klasifikasi langsung seperti pertanian, penebangan, atau pertambangan memerlukan validasi tambahan dan dapat ambigu.
- Tidak digunakan untuk penegakan hukum, klaim terhadap masyarakat, atau keputusan lingkungan nyata.

## Tujuan pembelajaran
- Memahami kelebihan dan keterbatasan sensor optik dan radar.
- Menunjukkan dampak awan pada ketersediaan data optik.
- Membuat aturan deteksi perubahan yang dapat diaudit.
- Memisahkan alert awal, kelas pola langsung, dan penyebab mendasar.
- Menjelaskan kebutuhan validasi lapangan.

## Metodologi
1. Buat lokasi sintetis dengan kondisi stabil atau berubah.
2. Simulasikan indikator optik sebelum/sesudah serta kemungkinan awan.
3. Simulasikan indikator radar yang tetap tersedia saat optik tertutup awan.
4. Hitung skor perubahan dan keluarkan alert awal.
5. Bandingkan hasil dengan label simulasi dan diskusikan false positive/false negative.

## Menjalankan
```bash
pip install -r ../requirements.txt
jupyter lab
```
Buka `studi_kasus_06_remote_sensing.ipynb` dan pilih **Run All**.

