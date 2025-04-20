## 📌 Type 1 Error dan Type 2 Error dalam Uji Hipotesis

Dalam **statistik inferensial**, saat kita melakukan **uji hipotesis** untuk menguji suatu klaim atau pernyataan mengenai populasi, dua jenis kesalahan dapat terjadi. Kesalahan ini dikenal sebagai **Type 1 Error** dan **Type 2 Error**. Kedua jenis kesalahan ini juga berlaku dalam uji hipotesis yang menggunakan **Student T Distribution** dan **Z-test**, meskipun ada sedikit perbedaan dalam cara keduanya diterapkan tergantung pada kondisi data dan asumsi.

### ⚖️ Apa Itu Type 1 Error dan Type 2 Error?

#### 1. **Type 1 Error (Kesalahan Tipe I)**:
- **Definisi**: Type 1 Error terjadi ketika kita **salah menolak hipotesis nol (H₀)**, yang berarti kita **menyimpulkan bahwa ada perbedaan atau hubungan**, padahal kenyataannya **tidak ada perbedaan atau hubungan**. Dengan kata lain, kita menganggap ada efek yang signifikan meskipun tidak ada, atau kita mengatakan bahwa hipotesis nol salah padahal sebenarnya benar.
  
- **Contoh**: 
  Misalnya, kita ingin menguji apakah rata-rata nilai ujian siswa lebih besar dari **75**. Hipotesis nol (H₀) menyatakan bahwa rata-rata nilai siswa **sama dengan 75**. Jika kita melakukan uji hipotesis dan mendapatkan nilai p yang sangat kecil (misalnya p < 0,05), kita **menolak hipotesis nol** dan menyimpulkan bahwa rata-rata nilai lebih besar dari 75. Namun, jika ternyata rata-rata sebenarnya **adalah 75**, kita telah melakukan **Type 1 Error**, yaitu salah menolak hipotesis nol yang benar.

- **Tingkat Signifikansi (α)**:
  - **Type 1 Error** berkaitan dengan **tingkat signifikansi (α)** dalam uji hipotesis, yang biasanya ditentukan sebelumnya oleh peneliti. Misalnya, jika α = 0,05, ini berarti ada kemungkinan **5%** kesalahan Type 1 yang dapat diterima.
  - **P-value** yang dihasilkan dari uji hipotesis digunakan untuk mengukur kemungkinan terjadinya Type 1 Error. Jika p-value lebih kecil dari α, kita akan menolak hipotesis nol, dan semakin kecil p-value, semakin besar kemungkinan kita telah melakukan **Type 1 Error**.

#### 2. **Type 2 Error (Kesalahan Tipe II)**:
- **Definisi**: Type 2 Error terjadi ketika kita **salah gagal menolak hipotesis nol (H₀)**, yang berarti kita **tidak menyimpulkan adanya perbedaan atau hubungan**, padahal kenyataannya **ada perbedaan atau hubungan**. Dengan kata lain, kita gagal untuk mendeteksi efek yang sebenarnya ada. Ini adalah kesalahan di mana kita **menganggap hipotesis nol benar padahal sebenarnya salah**.
  
- **Contoh**: 
  Misalnya, kita menguji apakah rata-rata nilai ujian siswa lebih besar dari **75**, tetapi setelah analisis, kita **tidak menolak hipotesis nol** dan menyimpulkan bahwa rata-rata nilai **sama dengan 75**. Padahal, sebenarnya rata-rata nilai siswa **lebih besar dari 75**. Dalam hal ini, kita telah melakukan **Type 2 Error**, yaitu gagal untuk mendeteksi perbedaan yang sebenarnya ada.

- **Kekuatan Uji (Power)**:
  - **Type 2 Error** berkaitan dengan **kekuatan uji** (power of the test), yang mengukur kemampuannya untuk mendeteksi perbedaan yang ada jika memang ada. Semakin tinggi **kekuatan uji**, semakin kecil kemungkinan kita melakukan **Type 2 Error**.
  - Faktor-faktor yang memengaruhi **kekuatan uji** termasuk ukuran sampel, variasi dalam data, dan **tingkat signifikansi (α)** yang digunakan. Semakin besar ukuran sampel dan semakin kecil variasi data, semakin besar kemungkinan uji untuk mendeteksi perbedaan yang ada, sehingga mengurangi risiko **Type 2 Error**.

---

### 📉 Perbedaan Antara Type 1 dan Type 2 Error

| **Kesalahan**               | **Type 1 Error (Kesalahan Tipe I)**              | **Type 2 Error (Kesalahan Tipe II)**              |
|-----------------------------|-------------------------------------------------|-------------------------------------------------|
| **Deskripsi**               | Menyimpulkan bahwa ada perbedaan/pengaruh, padahal tidak ada (salah menolak H₀) | Menyimpulkan bahwa tidak ada perbedaan/pengaruh, padahal ada (salah gagal menolak H₀) |
| **Contoh Kasus**            | Menyimpulkan bahwa rata-rata nilai ujian lebih tinggi dari 75, padahal sebenarnya 75 | Menyimpulkan bahwa rata-rata nilai ujian sama dengan 75, padahal sebenarnya lebih tinggi dari 75 |
| **Tingkat Signifikansi (α)**| Merupakan probabilitas melakukan **Type 1 Error** (misalnya, 0,05) | Merupakan probabilitas melakukan **Type 2 Error** (berkaitan dengan kekuatan uji) |
| **Faktor yang Mempengaruhi**| Menurunkan α (misalnya, α = 0,01) mengurangi **Type 1 Error**, tetapi dapat meningkatkan **Type 2 Error** | Menambah ukuran sampel, mengurangi variasi, atau meningkatkan tingkat signifikansi (α) dapat mengurangi **Type 2 Error** |
| **Pengaruh pada Keputusan** | Mengambil keputusan yang salah karena menilai ada efek yang sebenarnya tidak ada | Gagal mengambil keputusan yang benar karena tidak mendeteksi efek yang ada |

---

### 📊 Bagaimana Type 1 dan Type 2 Error Terjadi pada Student T-Distribution vs Z-Test?

- **Pada Z-test**:
  - **Type 1 Error**: Terjadi ketika kita menolak hipotesis nol yang sebenarnya benar. Ini biasanya terjadi ketika sampel cukup besar dan simpangan baku populasi diketahui.
  - **Type 2 Error**: Terjadi ketika kita gagal menolak hipotesis nol meskipun hipotesis alternatif benar, ini lebih sering terjadi ketika ukuran sampel kecil atau variasi data sangat tinggi.
  
- **Pada Student T-Distribution**:
  - **Type 1 Error**: Terjadi ketika kita menolak hipotesis nol yang benar meskipun ukuran sampel kecil dan simpangan baku populasi tidak diketahui.
  - **Type 2 Error**: Pada distribusi t, **Type 2 Error** lebih mungkin terjadi pada sampel kecil, karena ketidakpastian lebih besar yang ditimbulkan oleh **ekor distribusi t yang lebih tebal**.

---

### 🧠 Kesimpulan

- **Type 1 Error (Kesalahan Tipe I)** terjadi ketika kita **salah menolak hipotesis nol** yang benar (menyimpulkan ada perbedaan/pengaruh padahal tidak ada).
- **Type 2 Error (Kesalahan Tipe II)** terjadi ketika kita **gagal menolak hipotesis nol** yang salah (menganggap tidak ada perbedaan/pengaruh padahal ada).
- Dalam **Z-test** dan **Student T-Distribution**, kedua jenis kesalahan ini dapat terjadi tergantung pada **ukuran sampel**, **simpangan baku**, dan **tingkat signifikansi (α)** yang digunakan.
- Untuk **mengurangi Type 1 Error**, kita dapat menurunkan nilai α, tetapi ini bisa meningkatkan **Type 2 Error**. Sebaliknya, **meningkatkan ukuran sampel** dapat membantu mengurangi **Type 2 Error**.

---

### 📚 Referensi

1. Rumsey, D. (2016). *Statistics for Dummies* (2nd ed.). Wiley.  
2. Walpole, R. E., Myers, R. H., Myers, S. L., & Ye, K. (2012). *Probability and Statistics for Engineers and Scientists* (9th ed.). Pearson.  
3. Laerd Statistics. [T-Distribution Guide](https://statistics.laerd.com/statistical-guides/t-distribution-statistical-guide.php)  
4. Laerd Statistics. [Z-Test Guide](https://statistics.laerd.com/statistical-guides/z-test-statistical-guide.php)
