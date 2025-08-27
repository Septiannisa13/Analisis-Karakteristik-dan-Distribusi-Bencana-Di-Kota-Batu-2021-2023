# 📊 **Analisis Faktor Kecelakaan Lalu Lintas untuk Optimalisasi Keselamatan Pengguna Jalan** 📊
**Sumber Data:** BPBD Kota Batu
**Periode Data:** 2021-2023
**Pemrosesan Data:** Data dikompilasi menjadi dataset gabungan yang mencakup kejadian bencana selama tiga tahun untuk mendukung analisis lanjutan.

## 📖 **Deskripsi Proyek**
Dataset ini berisi informasi bencana yang terjadi di Kota Batu selama periode 2021–2023. Data bersumber dari Badan Penanggulangan Bencana Daerah (BPBD) Kota Batu dan telah diolah untuk memberikan gambaran yang lebih komprehensif mengenai pola dan sebaran bencana di wilayah tersebut. Dataset ini mencakup berbagai jenis bencana di tiap desa/kelurahan, lengkap dengan koordinat geografis setiap lokasi, sehingga mendukung analisis geospasial dan perencanaan mitigasi bencana yang lebih efektif.

## 📊 **Struktur Dataset**
Kolom	Deskripsi
Desa/Kelurahan	Nama desa atau kelurahan tempat terjadinya bencana
Kecamatan	Nama kecamatan di Kota Batu
Latitude	Koordinat lintang desa/kelurahan
Longitude	Koordinat bujur desa/kelurahan
Banjir	Jumlah kejadian banjir di desa/kelurahan tersebut
Tanah Longsor	Jumlah kejadian tanah longsor di desa/kelurahan tersebut
Cuaca Ekstrem	Jumlah kejadian akibat cuaca ekstrem
Kebakaran Hutan dan Lahan	Jumlah kejadian kebakaran hutan dan lahan
Gempa Bumi	Jumlah kejadian gempa bumi yang memengaruhi wilayah tersebut
Erupsi Gunung Api	Jumlah kejadian erupsi gunung api
Epidemi dan Wabah Penyakit	Jumlah kejadian epidemi atau wabah penyakit yang tercatat
Gagal Teknologi	Jumlah kejadian yang berkaitan dengan kegagalan teknologi
Konflik Sosial	Jumlah kejadian konflik sosial
Total	Jumlah keseluruhan kejadian bencana di desa/kelurahan tersebut

Setiap kolom di atas menggambarkan jenis dan frekuensi bencana di masing-masing wilayah. Kolom Total merangkum seluruh kejadian bencana, memberikan gambaran menyeluruh mengenai tingkat kerentanan setiap desa atau kelurahan.

## 🔍 **Metodologi Proyek**
1. 🔄 **Preprocessing Data:**
- Data Cleaning: Menghapus nilai yang hilang atau tidak relevan.
- Data Reduction: Menggunakan feature selection untuk mengurangi jumlah fitur yang digunakan dalam model.
- Data Transformation: Mengonversi data kategorik menjadi numerik.
- Data Normalization: Menerapkan skala Min-Max pada data numerik agar bernilai antara 0 hingga 1.
2. ⚛️ **Algoritma Klasifikasi:**
  Model utama yang digunakan dalam analisis ini adalah Gradient Boosting Classifier, yang terbukti memberikan akurasi tinggi. Selain itu, percobaan dilakukan dengan lima algoritma lainnya untuk memastikan keakuratan model.
3. 💡 **Oversampling & Balancing:**
 Menggunakan teknik SMOTEENN untuk menangani ketidakseimbangan kelas dalam data, yang meningkatkan akurasi prediksi model.

## 📝 **Analisis Hasil**
1. Model Akurasi: Model Gradient Boosting dengan Hyperparameter Tuning menunjukkan akurasi sebesar 81%.
2. Feature Importance: Fitur Age_band_of_driver (kelompok umur pengemudi) dan Educational_level (tingkat pendidikan) menunjukkan pengaruh yang signifikan dalam menentukan tingkat keparahan kecelakaan.
3. Confusion Matrix:
- Kelas 0 (Ringan): Mengalami kesulitan dalam mengidentifikasi kasus dengan tepat.
- Kelas 1 (Sedang): Hanya 15 dari 284 kasus diprediksi dengan benar.
- Kelas 2 (Fatal): Model berhasil memprediksi 1.613 dari 2.018 kasus dengan benar.

## 📈 **Visualisasi Hasil**
Hasil analisis ditampilkan melalui Confusion Matrix dan grafik tingkat kepentingan fitur. Visualisasi ini memberikan gambaran fitur mana yang paling berperan dalam memprediksi tingkat keparahan kecelakaan.

## 📂 **Kesimpulan**
Analisis menunjukkan bahwa kesalahan manusia—terutama yang berkaitan dengan usia dan tingkat pendidikan pengemudi yang menjadi faktor utama penyebab kecelakaan lalu lintas. Temuan ini diharapkan dapat mendukung pihak berwenang dan masyarakat dalam merumuskan strategi guna meningkatkan keselamatan berkendara.
