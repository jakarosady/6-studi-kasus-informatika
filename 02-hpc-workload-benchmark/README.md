# Studi Kasus 2 — Benchmark Komputasi dan Pemecahan Masalah Skala Besar

![HPC](https://img.shields.io/badge/Topik-HPC%20dan%20benchmark-purple) ![Notebook](https://img.shields.io/badge/Format-ipynb-orange)

## Ringkasan
Materi kedua membahas High Performance Computing (HPC), FLOPS, infrastruktur komputasi, dan jembatan antara tantangan lokal dengan kemampuan komputasi berskala besar. Proyek ini membuat eksperimen **Monte Carlo untuk mengestimasi π** sebagai contoh beban kerja yang dapat dibagi menjadi potongan independen.

## Studi kasus
Sebuah tim riset ingin memperkirakan konstanta π menggunakan simulasi acak. Tim perlu memahami:
- bagaimana pendekatan statistik sederhana menghasilkan estimasi;
- bagaimana jumlah sampel memengaruhi galat;
- bagaimana pembagian pekerjaan dan overhead memengaruhi waktu eksekusi;
- mengapa benchmark perlu dilakukan secara adil.

## Batasan masalah
- Notebook berjalan di mesin lokal; ini bukan demonstrasi akses ke superkomputer atau GPU cluster.
- Waktu benchmark tidak dapat dibandingkan lintas perangkat tanpa kontrol lingkungan.
- `ThreadPoolExecutor` dapat lebih lambat untuk komputasi CPU-bound di CPython karena overhead dan Global Interpreter Lock (GIL).
- Estimasi Monte Carlo bersifat stokastik; hasil berubah menurut seed dan jumlah sampel.
- Contoh ini tidak digunakan untuk keputusan ilmiah kritis.

## Tujuan pembelajaran
- Menghubungkan masalah komputasi dengan desain eksperimen.
- Mengukur waktu, jumlah pekerjaan, dan galat estimasi.
- Menjelaskan speedup dan efisiensi tanpa mengasumsikan paralelisme selalu menguntungkan.
- Mengidentifikasi kapan diperlukan infrastruktur HPC, optimasi algoritma, atau komputasi terdistribusi.

## Metodologi
1. Jalankan simulasi Monte Carlo dengan seed tetap.
2. Bandingkan estimasi untuk beberapa ukuran sampel.
3. Ukur waktu beberapa konfigurasi eksekusi.
4. Hitung speedup relatif terhadap baseline.
5. Diskusikan faktor yang membatasi interpretasi benchmark.

## Menjalankan
```bash
pip install -r ../requirements.txt
jupyter lab
```
Buka `studi_kasus_02_hpc_benchmark.ipynb` dan pilih **Run All**.


