# Studi Kasus 1 — Audit Kualitas Data dan Analitik Penjualan

![Python](https://img.shields.io/badge/Python-3.10%2B-blue) ![Jupyter](https://img.shields.io/badge/Notebook-ipynb-orange) ![Data](https://img.shields.io/badge/Data-sintetis-lightgrey)

## Ringkasan
Studi ini menerjemahkan gagasan dari materi **Make Sense of Data with Analysis and AI**: data nyata sering berantakan, sehingga keputusan berbasis data harus diawali pemeriksaan kualitas. Notebook membangun contoh data transaksi distributor, mengaudit nilai kosong/duplikat/format, membersihkan data, lalu menghitung KPI dan tren.

## Studi kasus dan rumusan masalah
Distributor fiktif menerima transaksi dengan format tanggal tidak seragam, kuantitas kosong, baris duplikat, dan harga tidak valid. Pertanyaan yang dijawab:
1. Masalah kualitas data apa yang ditemukan?
2. Berapa pendapatan bersih setelah aturan pembersihan diterapkan?
3. Produk dan bulan mana yang paling berkontribusi?
4. Baris mana yang perlu ditinjau, bukan otomatis dihapus?

## Batasan masalah
- Dataset dibuat secara sintetis dan hanya untuk pembelajaran.
- Pendapatan dihitung sebagai `kuantitas × harga_satuan`; diskon, pajak, retur, dan biaya operasional tidak dimodelkan.
- Pencilan ditandai dengan aturan IQR untuk ditinjau manusia, bukan dianggap pasti salah.
- Korelasi atau tren tidak membuktikan hubungan sebab-akibat.
- Tidak ada model machine learning yang dipakai untuk membuat keputusan bisnis otomatis.

## Tujuan pembelajaran
- Memahami bahwa kualitas data memengaruhi kualitas analisis.
- Menggunakan `pandas` untuk audit dan transformasi data.
- Menghasilkan KPI yang bisa ditelusuri kembali ke data sumber.
- Menjelaskan asumsi dan batas interpretasi hasil.

## Metodologi
1. Buat data contoh dengan masalah kualitas yang disengaja.
2. Audit bentuk data, tipe, nilai kosong, duplikasi, dan nilai tidak masuk akal.
3. Bersihkan menggunakan aturan eksplisit dan dokumentasikan baris yang dibuang.
4. Hitung pendapatan dan agregasi per bulan/produk.
5. Tandai pencilan untuk pemeriksaan lanjutan.

## Menjalankan notebook
```bash
python -m venv .venv
# Windows: .venv\\Scripts\\activate
# macOS/Linux: source .venv/bin/activate
pip install -r ../requirements.txt
jupyter lab
```
Buka `studi_kasus_01_analitik_data.ipynb`, lalu pilih **Run All**.

## Kriteria keberhasilan
- Notebook berjalan dari atas ke bawah.
- Aturan pembersihan dapat dijelaskan dan tidak disembunyikan.
- Angka KPI berasal dari data bersih.
- Temuan menyebutkan keterbatasan dataset.

## Struktur
- `studi_kasus_01_analitik_data.ipynb` — proses audit dan analisis.
- `README.md` — penjelasan kasus dan batasan.
