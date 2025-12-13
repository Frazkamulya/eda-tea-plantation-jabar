# Exploratory Data Analysis: Luas Tanaman Teh Jawa Barat (2013–2024)

Project ini bertujuan untuk melakukan Exploratory Data Analysis (EDA) terhadap dataset komoditas tanaman tahunan teh di Provinsi Jawa Barat.  
Analisis difokuskan pada pola luas tanaman berdasarkan:
- Kabupaten/Kota
- Kondisi tanaman (TBM, TM, TR/TTM)
- Perubahan luas tanaman per tahun
- Distribusi keseluruhan luas tanaman

Dataset bersumber dari Open Data Jabar dan mencakup tahun 2013–2024, sehingga cocok untuk analisis tren jangka panjang.

---

## Dataset
Sumber: Open Data Jabar  
https://opendata.jabarprov.go.id/

Kolom dalam dataset:
- kode_provinsi
- nama_provinsi
- kode_kabupaten_kota
- nama_kabupaten_kota
- kondisi_tanaman
- tbm (tanaman belum menghasilkan)
- tm (tanaman menghasilkan)
- tr/ttm (rusak / tidak menghasilkan)
- luas_tanaman
- satuan
- tahun

Format: CSV  
Lokasi file: folder /data

---

## Tools dan Libraries
- Python
- Jupyter Notebook
- pandas
- matplotlib
- seaborn

---

## Struktur Project

(Project structure ditampilkan di repository)

---

## Hasil Exploratory Data Analysis (EDA)

### 1. Data Quality Check
- Tidak terdapat missing values
- Tidak terdapat data duplikat
- Tipe data sudah sesuai (tahun sebagai integer, luas_tanaman sebagai numerik)
- Dataset siap digunakan tanpa proses pembersihan lanjutan

---

## Insight EDA (Temuan Utama)

1. Distribusi luas_tanaman bersifat right-skewed, menunjukkan sebagian besar kabupaten/kota memiliki luas lahan kecil hingga menengah, sementara hanya beberapa daerah dengan luas lahan sangat besar.
2. Kontribusi luas tanaman tidak merata dan terpusat pada beberapa kabupaten tertentu.
3. Perubahan luas tanaman per tahun menunjukkan pola fluktuatif yang mengindikasikan dinamika penggunaan lahan.
4. Kondisi tanaman TM (Tanaman Menghasilkan) mendominasi, menandakan sebagian besar lahan berada pada fase produktif.
5. Nilai TR/TTM yang cukup besar di beberapa wilayah mengindikasikan adanya penurunan produktivitas atau kerusakan lahan.
6. TBM mencerminkan proses regenerasi kebun, yang berpotensi meningkatkan produksi di masa depan.
7. Terdapat perbedaan signifikan antar daerah, sehingga pendekatan kebijakan sebaiknya disesuaikan secara lokal.
8. Satuan data sudah konsisten dan standar (hektar), sehingga memudahkan analisis lanjutan.

---

## Storytelling Analisis

Perkebunan teh merupakan salah satu komoditas penting di Jawa Barat. Dataset yang mencakup periode 2013 hingga 2024 memberikan gambaran jangka panjang mengenai perubahan luas lahan perkebunan teh di berbagai wilayah.

Analisis dimulai dari pemeriksaan kualitas data yang menunjukkan dataset berada dalam kondisi baik. Distribusi luas tanaman memperlihatkan bahwa sebagian besar produksi terkonsentrasi pada beberapa kabupaten tertentu, menandakan struktur industri yang tidak merata.

Tren tahunan memperlihatkan adanya kenaikan dan penurunan luas tanaman yang mencerminkan pengaruh faktor eksternal seperti kebijakan, kondisi lingkungan, serta peremajaan tanaman. Analisis kondisi tanaman memperkuat pemahaman mengenai fase produksi, regenerasi, dan potensi penurunan produktivitas di beberapa wilayah.

Hasil analisis ini relevan bagi pemerintah daerah maupun pelaku industri sebagai dasar pengambilan keputusan berbasis data.

---

## Kesimpulan

1. Luas tanaman teh di Jawa Barat tidak terdistribusi secara merata.
2. Terdapat fluktuasi tahunan yang mencerminkan dinamika industri perkebunan.
3. Kondisi tanaman menunjukkan kombinasi antara lahan produktif dan area yang memerlukan perhatian khusus.
4. Dataset memiliki kualitas baik dan layak untuk analisis lanjutan.
5. Analisis lanjutan seperti peramalan atau analisis spasial sangat memungkinkan dilakukan.

---

## Rekomendasi Analitis

Untuk Pemerintah dan Industri:
- Perlu fokus pada wilayah dengan nilai TR/TTM tinggi untuk menekan lahan tidak produktif.
- Evaluasi kebijakan diperlukan pada daerah dengan tren luas tanaman menurun.
- Wilayah dengan nilai TBM besar berpotensi menjadi pusat produksi di masa depan.

Untuk Pengembangan Analisis:
- Menambahkan data produksi, harga, dan luas panen.
- Melakukan forecasting menggunakan metode time series.
- Mengembangkan analisis spasial jika data geografis tersedia.

---

## Cara Menjalankan Project

1. Clone repository
2. Install dependencies
3. Jalankan file eda.ipynb di Jupyter Notebook
4. Analisis dan visualisasi dapat dilihat langsung di notebook

---

## Author
Nama: Frazka Mulya Wijaya  
Role: Data Analyst / Data Science Enthusiast
