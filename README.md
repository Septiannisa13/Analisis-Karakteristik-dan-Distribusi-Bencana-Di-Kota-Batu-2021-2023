# 📊 **Analisis Karakteristik dan Distribusi Bencana Di Kota Batu 2021-2023** 📊
**Sumber Data:** BPBD Kota Batu
**Periode Data:** 2021-2023
**Pemrosesan Data:** Data dikompilasi menjadi dataset gabungan yang mencakup kejadian bencana selama tiga tahun untuk mendukung analisis lanjutan.

## 📖 **Deskripsi Proyek**
Dataset ini berisi informasi bencana yang terjadi di Kota Batu selama periode 2021–2023. Data bersumber dari Badan Penanggulangan Bencana Daerah (BPBD) Kota Batu dan telah diolah untuk memberikan gambaran yang lebih komprehensif mengenai pola dan sebaran bencana di wilayah tersebut. Dataset ini mencakup berbagai jenis bencana di tiap desa/kelurahan, lengkap dengan koordinat geografis setiap lokasi, sehingga mendukung analisis geospasial dan perencanaan mitigasi bencana yang lebih efektif.

## 📊 **Struktur Dataset**
Dataset ini berisi informasi bencana di tiap desa atau kelurahan di Kota Batu. Kolom Desa/Kelurahan mencatat nama wilayah tempat bencana terjadi, sedangkan Kecamatan menunjukkan kecamatan terkait. Latitude dan Longitude memberikan koordinat geografis lokasi tersebut.

Kolom bencana mencatat jumlah kejadian untuk setiap jenis bencana, seperti banjir, tanah longsor, cuaca ekstrem, kebakaran hutan dan lahan, gempa bumi, erupsi gunung api, epidemi dan wabah penyakit, gagal teknologi, dan konflik sosial.

Kolom Total merangkum seluruh kejadian bencana di suatu desa atau kelurahan, sehingga memberikan gambaran umum tentang tingkat kerentanan wilayah tersebut.

## 🔍 **Metodologi Proyek**
1. **Data Loading**
Skrip ini memuat dataset mentah dari BPBD dan menyiapkannya untuk analisis lebih lanjut.
2. **Data Preprocessing**
Menggunakan StandardScaler untuk normalisasi data, sehingga seluruh nilai berada dalam skala yang seragam, yang memudahkan analisis dan mengurangi bias dalam klasterisasi.
3. **Clustering**
 Menggunakan algoritma KMeans untuk mengelompokkan data berdasarkan lokasi atau jenis bencana. Pengelompokan ini dapat membantu dalam mengidentifikasi pola wilayah yang paling rawan atau jenis bencana tertentu yang lebih sering terjadi di lokasi tertentu.
4. **PCA (Principal Component Analysis)**
Menggunakan PCA untuk mereduksi dimensi data, memungkinkan visualisasi data dalam ruang berdimensi rendah, yang memudahkan pemahaman pola distribusi bencana secara keseluruhan.

## 📝 **Tujuan Proyek**
Dataset dan skrip ini dapat digunakan untuk berbagai tujuan, antara lain:
- Perencanaan Mitigasi dan Kesiapsiagaan: Membantu pihak BPBD dan pemerintah daerah dalam merencanakan langkah mitigasi di wilayah-wilayah rawan bencana.
- Penelitian Akademik: Dataset ini juga dapat menjadi dasar bagi peneliti yang ingin mengembangkan studi lebih lanjut terkait mitigasi bencana atau analisis spasial di bidang kebencanaan.

## 📂 **Kesimpulan**
Dataset ini tersedia untuk kepentingan penelitian, analisis, dan perencanaan mitigasi bencana. Harap menyertakan atribusi kepada BPBD Kota Batu jika dataset ini digunakan dalam publikasi atau penelitian.
