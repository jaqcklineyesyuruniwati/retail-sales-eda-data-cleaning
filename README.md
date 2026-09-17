# 🛒 Terbimbing: Eksplorasi Data & Cleaning Dataset Ritel (EDA)

Proyek terbimbing ini berfokus pada penerapan siklus *Exploratory Data Analysis* (EDA) secara sistematis dan terstruktur menggunakan bahasa pemrograman Python. Studi kasus menggunakan dataset penjualan ritel (`retail_sales.csv`) yang mencakup alur kerja dari pemuatan data mentah hingga penyusunan kesimpulan bisnis.

---

## 📂 Alur Kerja Proyek (Step-by-Step)

1. **Setup & Lingkungan Kerja:** Mengimpor pustaka utama (`pandas`, `numpy`, `matplotlib`, `seaborn`), mengatur konfigurasi `%matplotlib inline`, dan menetapkan gaya visual `whitegrid`.
2. **Memuat Dataset:** Memuat file `retail_sales.csv` ke dalam Pandas DataFrame dan memverifikasi kolom utamanya.
3. **Inspeksi Awal:** Memeriksa struktur dataset menggunakan `df.info()` dan melihat ringkasan statistik menggunakan `df.describe()`.
4. **Analisis Missing Value:** Menghitung jumlah dan persentase nilai kosong secara presisi (`isnull().sum()`) pada kolom `CustomerID` dan `Description`.
5. **Pembersihan Data (Data Cleaning):** Menerapkan strategi penanganan nilai kosong menggunakan metode yang sesuai serta menyalin data ke `df_clean` untuk mencegah peringatan *SettingWithCopyWarning*.
6. **Visualisasi Data & EDA:**
   * **Histogram:** Menganalisis distribusi jumlah pembelian (`Quantity`) yang bersifat *right-skewed*.
   * **Boxplot & IQR:** Mengidentifikasi sebaran harga satuan (`UnitPrice`) dan menyaring *outlier* ekstrem menggunakan aturan rentang interkuartil (IQR).
   * **Scatter Plot:** Mengeksplorasi hubungan antara kuantitas pembelian dan harga satuan.
   * **Heatmap Korelasi:** Mengukur kekuatan hubungan linear antar-variabel numerik secara kuantitatif.
7. **Analisis Kategorik:** Menampilkan sepuluh negara dengan transaksi terbanyak menggunakan diagram batang `.value_counts()`.

---

## 🛠️ Tech Stack
* **Python**
* **Pandas & NumPy** (Manipulasi & Pembersihan Data)
* **Matplotlib & Seaborn** (Visualisasi Data Lanjutan)

---

## 💡 Temuan & Kesimpulan Utama
* Sebagian besar transaksi pembelian terkonsentrasi pada kuantitas kecil (1–10 unit).
* Terdapat *outlier* nilai ekstrem pada harga satuan (*UnitPrice*).
* Hubungan linear antara kuantitas pembelian dan harga satuan tergolong lemah berdasarkan *scatter plot* dan *heatmap* korelasi.
* Negara asal toko (*United Kingdom*) mendominasi volume transaksi secara signifikan.

---

## 🚀 Cara Menjalankan
1. Pastikan file dataset `retail_sales.csv` berada dalam satu direktori dengan notebook.
2. Buka file `.ipynb` menggunakan **Jupyter Notebook** atau **Google Colab**.
3. Jalankan sel kode secara berurutan.
