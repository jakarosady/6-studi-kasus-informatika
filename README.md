# 6 Studi Kasus Informatika — Notebook Python, Analisis, dan GitHub

![Python](https://img.shields.io/badge/Python-3.10%2B-blue) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange) ![Status](https://img.shields.io/badge/status-edukasi-informational)


## Daftar isi
1. [Audit Kualitas Data dan Analitik Penjualan](#1-audit-kualitas-data-dan-analitik-penjualan)
2. [Benchmark Komputasi dan HPC](#2-benchmark-komputasi-dan-hpc)
3. [Prioritas Inspeksi Aset Berbasis GIS](#3-prioritas-inspeksi-aset-berbasis-gis)
4. [Klasifikasi Risiko Keterlambatan dengan ML](#4-klasifikasi-risiko-keterlambatan-dengan-ml)
5. [Audit Usability Portal Akademik](#5-audit-usability-portal-akademik)
6. [Deteksi Perubahan Hutan Multi-Sensor](#6-deteksi-perubahan-hutan-multi-sensor)

## Pemetaan materi ke studi kasus

| Urutan | Materi sumber yang tersedia | Studi kasus implementasi |
|---|---|---|
| 1 | Andrea Arisal — *Make Sense of Data with Analysis and AI* (`WeIWNNO5vbk.txt`) | Audit data transaksi dan analitik penjualan |
| 2 | Dr. Warawan Diaz Carbalo — HPC dan tantangan lokal (`qeWpf9uXBqE.txt`) | Simulasi Monte Carlo dan benchmark lokal |
| 3 | Widi Primadepa — karier industri dengan GIS (`TkXkx7HKTto.txt`) | Prioritas inspeksi aset menggunakan koordinat |
| 4 | Materi pengantar Machine Learning (`0LFeuSypYro.txt`) | Klasifikasi risiko keterlambatan pada data sintetis |
| 5 | Dokumen Modul IMK (`TRANSKRIP SESI 5.docx`) | Audit usability, persona, kebutuhan, dan metrik |
| 6 | Dr. Bart Slachter — remote sensing dan deforestation alerts (`Informatika S1's Zoom Meeting.txt`) | Deteksi perubahan hutan multi-sensor sintetis |

**Catatan pemetaan sumber:** nama berkas yang diunggah tidak seluruhnya identik dengan ID tautan video. Pemetaan di atas mengikuti isi berkas yang tersedia dan urutan yang diinformasikan pengguna. Berkas `TRANSKRIP SESI 5.docx` berupa ringkasan enam modul IMK, bukan transkrip dialog video. Topik remote sensing berasal dari berkas `Informatika S1's Zoom Meeting.txt`. Jika berkas tersebut seharusnya mewakili urutan tautan yang berbeda, sesuaikan pemetaan sebelum publikasi.

## 1. Audit Kualitas Data dan Analitik Penjualan
Data transaksi sintetis berisi nilai kosong, duplikasi, tanggal invalid, dan harga tidak valid. Notebook menunjukkan audit, aturan pembersihan, KPI, tren bulanan, serta pencilan yang perlu ditinjau.

## 2. Benchmark Komputasi dan HPC
Estimasi Monte Carlo untuk π digunakan sebagai contoh beban kerja komputasi. Notebook mengukur galat dan waktu lokal, lalu membahas speedup dan batasan threading. Ini bukan benchmark superkomputer.

## 3. Prioritas Inspeksi Aset Berbasis GIS
Aset sintetis diberi koordinat, kondisi, dan kritikalitas. Notebook menghitung jarak haversine, skor prioritas transparan, dan visualisasi sebaran. Tidak memakai jalan atau data GIS resmi.

## 4. Klasifikasi Risiko Keterlambatan dengan ML
Notebook menggunakan pipeline scikit-learn untuk preprocessing, train/test split, klasifikasi, confusion matrix, dan metrik precision/recall/F1. Dataset dan label bersifat sintetis.

## 5. Audit Usability Portal Akademik
Notebook membuat persona, kebutuhan, metrik success rate/task time, dan backlog temuan heuristik. Data pengujian bersifat sintetis, bukan hasil partisipan nyata atau audit WCAG formal.

## 6. Deteksi Perubahan Hutan Multi-Sensor
Notebook menyimulasikan indikator optik dan radar serta dampak observasi optik yang tertutup awan. Alert hanya demonstrasi perubahan; bukan pemetaan deforestasi aktual dan bukan penentuan sebab.

## Batasan umum paket
- Notebook adalah artefak pembelajaran dan tidak menggantikan analisis profesional.
- Dataset sintetis dipakai agar semua notebook bisa dijalankan tanpa unduhan eksternal atau data pribadi.
- Angka, label, dan hasil yang muncul merupakan hasil simulasi, bukan temuan lapangan.
- Tidak ada klaim bahwa pendekatan atau kode ini belum pernah ada di seluruh dunia. Paket dirancang khusus untuk enam kasus ini dan tidak menduplikasi studi kasus antarfolder.
- Untuk publikasi akademik, tambahkan identitas penulis, institusi, tanggal, serta sumber yang benar-benar digunakan sesuai aturan kampus.

## Prasyarat
- Python 3.10 atau lebih baru
- `pip`
- JupyterLab atau Jupyter Notebook
- Koneksi internet hanya diperlukan untuk instalasi dependensi awal (jika belum tersedia)

## Instalasi

### Windows (PowerShell)
```powershell
py -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
jupyter lab
```

### macOS/Linux
```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
jupyter lab
```

Buka notebook pada folder studi kasus yang diinginkan, lalu pilih **Run All**. Setiap notebook dibuat untuk berjalan dari atas ke bawah.

## Struktur repositori
```text
6-studi-kasus-informatika/
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
├── docs/
│   └── PANDUAN_UPLOAD_GITHUB.md
├── 01-analytics-data-ai/
│   ├── README.md
│   └── studi_kasus_01_analitik_data.ipynb
├── 02-hpc-workload-benchmark/
│   ├── README.md
│   └── studi_kasus_02_hpc_benchmark.ipynb
├── 03-gis-prioritas-aset/
│   ├── README.md
│   └── studi_kasus_03_gis_aset.ipynb
├── 04-machine-learning-risiko/
│   ├── README.md
│   └── studi_kasus_04_machine_learning.ipynb
├── 05-imk-usability/
│   ├── README.md
│   └── studi_kasus_05_imk_usability.ipynb
└── 06-remote-sensing-forest/
    ├── README.md
    └── studi_kasus_06_remote_sensing.ipynb
```

## Menambahkan hasil eksperimen
Jika mengubah data atau parameter:
1. Jalankan seluruh notebook dari awal.
2. Pastikan hasil sesuai dengan kode dan interpretasi.
3. Tambahkan konteks data, versi Python, dan batasan pada README.
4. Jangan mengunggah data rahasia, kredensial, atau data pribadi.
5. Periksa diff Git sebelum melakukan commit.

## Upload ke GitHub
Ikuti [panduan upload GitHub](docs/PANDUAN_UPLOAD_GITHUB.md).

## Lisensi dan atribusi
Kode dalam paket ini disediakan di bawah lisensi MIT. Materi seminar dan transkrip tetap milik pemateri/pemegang hak masing-masing; paket ini merangkum tema untuk latihan dan tidak mendistribusikan ulang transkrip lengkap. Cantumkan atribusi yang sesuai saat menggunakan atau mengembangkan paket.
