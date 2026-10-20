# Studi Kasus 3 — Prioritas Inspeksi Aset Berbasis GIS

![GIS](https://img.shields.io/badge/Topik-GIS%20%2F%20spasial-green) ![Notebook](https://img.shields.io/badge/Format-ipynb-orange)

## Ringkasan
Materi ketiga menyoroti karier GIS di industri, pengelolaan aset, pemetaan, analisis spasial, database, Python/SQL, web map, dan pentingnya menghubungkan pengetahuan informatika dengan kebutuhan operasional. Studi kasus ini membangun **prioritas inspeksi aset fasilitas** menggunakan data spasial sintetis.

## Rumusan masalah
Tim pemeliharaan memiliki aset yang tersebar di suatu wilayah. Waktu inspeksi terbatas, sehingga diperlukan daftar yang transparan untuk menentukan aset mana yang perlu diperiksa lebih dahulu.

Notebook:
- membuat aset sintetis dengan koordinat, kondisi, dan tingkat kritikalitas;
- menghitung jarak garis lurus dari depot;
- menyusun skor prioritas yang dapat diperiksa;
- menampilkan peta sebaran aset menggunakan grafik sederhana.

## Batasan masalah
- Semua lokasi merupakan koordinat sintetis, bukan lokasi fasilitas nyata.
- Jarak dihitung menggunakan rumus haversine; tidak mempertimbangkan jalan, lalu lintas, medan, atau akses masuk.
- Skor merupakan contoh pembobotan edukatif, bukan standar keselamatan.
- Tidak menggunakan data GIS resmi, citra drone, atau citra satelit.
- Keputusan akhir harus mempertimbangkan verifikasi lapangan, kondisi aktual, dan kebijakan organisasi.

## Tujuan
- Memahami representasi data spasial dalam tabel.
- Menghitung jarak geografis dengan koordinat lintang-bujur.
- Menggabungkan faktor kondisi dan jarak dalam aturan prioritas yang transparan.
- Menjelaskan manfaat sekaligus keterbatasan analisis GIS sederhana.

## Metodologi
1. Buat dataset aset dan satu depot.
2. Validasi rentang koordinat dan kelengkapan atribut.
3. Hitung jarak haversine.
4. Hitung skor prioritas berdasarkan kondisi dan kritikalitas.
5. Visualisasikan aset serta interpretasikan hasil dengan hati-hati.

## Menjalankan
```bash
pip install -r ../requirements.txt
jupyter lab
```
Buka `studi_kasus_03_gis_aset.ipynb` dan jalankan semua sel.


