# 📊 Exploratory Data Analysis: Luas Tanaman Teh Jawa Barat (2013–2024)

Project ini bertujuan untuk melakukan Exploratory Data Analysis (EDA) terhadap dataset komoditas tanaman tahunan *teh* di Provinsi Jawa Barat.  
Analisis difokuskan pada pola luas tanaman berdasarkan:
- Kabupaten/Kota  
- Kondisi tanaman (TBM, TM, TR/TTM)  
- Perubahan luas tanaman per tahun  
- Distribusi keseluruhan luas tanaman  

Dataset bersumber dari **Open Data Jabar** dan mencakup tahun **2013–2024**, sehingga sangat cocok untuk analisis tren jangka panjang.

---

## 📦 Dataset
**Sumber:** Open Data Jabar  
https://opendata.jabarprov.go.id/

**Kolom dalam dataset:**
- `kode_provinsi`  
- `nama_provinsi`  
- `kode_kabupaten_kota`  
- `nama_kabupaten_kota`  
- `kondisi_tanaman`  
- `tbm` (tanaman belum menghasilkan)  
- `tm` (tanaman menghasilkan)  
- `tr/ttm` (rusak / tidak menghasilkan)  
- `luas_tanaman`  
- `satuan`  
- `tahun`

Format: **CSV**  
Lokasi file: folder **/data**

---

## 🛠 Tools & Libraries

- Python  
- Jupyter Notebook  
- pandas  
- matplotlib  
- seaborn  

---

## 📁 Struktur Project


---

# 📈 Hasil Exploratory Data Analysis (EDA)

## ✔ 1. Data Quality Check
- Tidak ada missing values  
- Tidak ada duplikasi  
- Tipe data sudah sesuai (tahun = int, luas_tanaman = numeric)  
- Dataset siap dianalisis tanpa cleaning lanjutan  

---

# 🔍 **INSIGHT EDA (Temuan Utama)**

1. **Distribusi luas_tanaman bersifat right-skewed**, artinya sebagian besar kabupaten/kota memiliki lahan kecil–menengah, sementara segelintir daerah memiliki lahan sangat luas.  
2. **Kontribusi produksi tidak merata** — hanya beberapa kabupaten yang sangat dominan (misalnya Bandung, Cianjur, Garut, dll sesuai grafik).  
3. **Perubahan luas tanaman per tahun menunjukkan pola naik–turun**, mengindikasikan dinamika penggunaan lahan, kebijakan, dan produksi.  
4. **Kondisi tanaman TM (Tanaman Menghasilkan)** umumnya memiliki porsi terbesar, menandakan kebanyakan lahan sudah produktif.  
5. Jika **TR/TTM cukup besar**, ini mengindikasikan penurunan produktivitas atau kerusakan lahan.  
6. **TBM menunjukkan tingkat regenerasi perkebunan** — semakin besar TBM, semakin tinggi potensi produksi masa depan.  
7. Terdapat **perbedaan besar antar daerah**, menunjukkan kebutuhan strategi lokal khusus.  
8. Satuan data sudah standar (hektar), memudahkan perhitungan dan visualisasi.

---

# 🧠 **STORYTELLING (Narasi Analisis)**

Perkebunan teh di Jawa Barat merupakan salah satu komoditas penting di sektor pertanian. Dengan dataset yang berisi rangkaian data dari 2013 hingga 2024, analisis ini bertujuan memahami bagaimana perkembangan luas kebun teh berubah dari waktu ke waktu, serta bagaimana kondisi tanaman di berbagai wilayah.

Analisis dimulai dengan memastikan kualitas data—tidak ada nilai hilang atau duplikasi—yang membuat dataset ideal untuk dianalisis. Distribusi awal menunjukkan bahwa hanya sebagian kecil kabupaten/kota yang memegang peran besar dalam total luas tanaman teh. Hal ini berarti produksi sangat terpusat.

Visualisasi tren tahunan mengungkap bahwa perubahan luas tanaman tidak konstan—ada kenaikan dan penurunan yang mengindikasikan adanya faktor-faktor eksternal seperti cuaca, kebijakan, peremajaan tanaman, atau konversi lahan.

Ketika melihat kondisi tanaman (TBM, TM, TR/TTM), terlihat bagaimana kebun di tiap daerah berada dalam fase berbeda. TM menunjukkan produksi aktif, TBM menunjukkan regenerasi, sedangkan TR/TTM dapat menjadi indikator masalah yang perlu intervensi.

Temuan ini memberikan gambaran yang relevan untuk stakeholder pemerintah maupun industri dalam memahami dinamika perkebunan teh di Jawa Barat.

---

# 🏁 **Kesimpulan Utama**

1. Luas tanaman teh tidak merata dan terkonsentrasi di beberapa kabupaten.  
2. Tren tahunan menunjukkan fluktuasi signifikan yang mencerminkan perubahan industri.  
3. Kondisi tanaman menunjukkan adanya lahan produktif sekaligus area yang perlu perbaikan.  
4. Dataset berkualitas baik dan cocok untuk analisis lanjutan seperti forecasting.  
5. Ada peluang untuk analisis spasial atau prediksi jika data tambahan tersedia.

---

# 🚀 **Rekomendasi Analitis**

### 🔧 Untuk Pemerintah / Industri:
- Perlu perhatian khusus pada kabupaten dengan nilai **TR/TTM tinggi** untuk menekan jumlah lahan tidak produktif.  
- Daerah dengan tren luas tanaman **menurun** perlu evaluasi kebijakan penggunaan lahan.  
- Kabupaten dengan **TBM besar** berpotensi menjadi pusat produksi masa depan.  

### 📊 Untuk Analisis Lanjutan:
- Tambahkan data produksi (ton), harga, dan luas panen.  
- Lakukan forecasting produksi atau luas tanaman menggunakan ARIMA/Prophet.  
- Analisis spasial dengan peta jika data koordinat tersedia.

---

# 📌 Cara Menjalankan Project

1. Clone repository  
2. Install dependencies  
3. Jalankan `eda.ipynb` di Jupyter Notebook  
4. Lihat grafik dan insight langsung dari notebook  

---

# 👤 Author
Nama: **Frazka Mulya Wijaya**  
Role: Data Analyst / Data Science Enthusiast  
