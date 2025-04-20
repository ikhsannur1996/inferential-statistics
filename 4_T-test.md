## 📌 Apa Itu Distribusi T-Student dalam Uji Hipotesis?

### 🧠 Pengertian Umum

**Distribusi T-Student** adalah jenis distribusi probabilitas yang digunakan untuk menguji hipotesis ketika **simpangan baku populasi (σ)** tidak diketahui dan ukuran sampel **relatif kecil (n < 30)**. Distribusi ini sangat penting dalam statistik inferensial, terutama ketika data yang digunakan berasal dari sampel yang lebih kecil dan tidak dapat mengasumsikan distribusi normal sempurna.

Distribusi T-Student digunakan untuk mengestimasi **rata-rata populasi** dengan menggunakan **rata-rata sampel** dan **simpangan baku sampel (s)**. Dibandingkan dengan distribusi normal (Z-distribution), distribusi T-Student memiliki **ekor yang lebih tebal** untuk mengakomodasi variabilitas yang lebih besar dalam sampel kecil.

---

### 🧪 Kapan Distribusi T-Student Digunakan?

Distribusi T-Student digunakan ketika:
1. Ukuran sampel kecil (n < 30).
2. **Simpangan baku populasi (σ)** tidak diketahui.
3. Data yang diambil dianggap **berdistribusi normal**.
4. Uji yang dilakukan terkait dengan **rata-rata** (mean) populasi.

---

### 📐 Rumus T-Statistic

T-Statistic digunakan dalam uji hipotesis untuk membandingkan **rata-rata sampel** dengan **rata-rata populasi**. Rumusnya adalah:

![image](https://github.com/user-attachments/assets/84688a88-64c8-41ea-9168-59c6d4f5bd5a)


---

### 🔍 Penjelasan Sederhana

Bayangkan Anda adalah seorang dosen yang ingin mengetahui apakah nilai rata-rata ujian mahasiswa Anda berbeda dari nilai rata-rata ujian mahasiswa tahun lalu yang diketahui adalah **80**.

1. Anda mengambil sampel 15 mahasiswa dari kelas tahun ini.
2. Rata-rata nilai ujian sampel adalah **82**.
3. Anda tahu bahwa simpangan baku sampel adalah **10**.
4. Anda ingin tahu apakah perbedaan nilai tersebut **berarti secara statistik** atau hanya kebetulan.

Dengan menggunakan rumus **T-Statistic**, Anda bisa menghitung nilai **t** dan membandingkannya dengan **nilai kritis t** yang diperoleh dari **tabel distribusi T-Student** sesuai dengan **derajat kebebasan (degrees of freedom, df)** dan tingkat signifikansi (α) yang Anda tentukan.

---

### 📊 Interpretasi Hasil T-Student

Setelah nilai **t** dihitung, interpretasi hasil uji hipotesis adalah sebagai berikut:

1. **Tolak H₀** jika nilai t-hitung **lebih besar atau lebih kecil** dari nilai kritis t (tergantung jenis uji).
2. **Gagal menolak H₀** jika nilai t-hitung **terletak dalam wilayah netral**.

Contoh:
- t-hitung = 2.3
- t-kritis untuk α = 0.05 (two-tailed) dengan df = 14 adalah ±2.144
- Karena 2.3 > 2.144 → **Tolak H₀** → Ada perbedaan signifikan

---

### 🧾 Contoh Kasus Sederhana

**Masalah**: Seorang peneliti ingin mengetahui apakah rata-rata waktu tidur mahasiswa berbeda dari 7 jam per malam.

- Rata-rata waktu tidur yang dihipotesiskan: 7 jam
- Sampel 12 mahasiswa, rata-rata waktu tidur: 6.5 jam
- Simpangan baku sampel: 1 jam
- α = 0.05

**Langkah-langkah**:
1. Rumus T-Statistic:
![image](https://github.com/user-attachments/assets/e1e2dc24-6d00-4135-90c5-64818e7bf304)

2. t-kritis untuk uji dua sisi (α = 0.05) dan df = 11 adalah ±2.201.
3. Karena -1.73 berada dalam wilayah netral → **Gagal menolak H₀**

**Kesimpulan**: Tidak cukup bukti untuk menyatakan bahwa rata-rata waktu tidur mahasiswa berbeda secara signifikan dari 7 jam per malam.

---

### 🧠 Perbedaan T-Distribution dan Z-Distribution

| Aspek                  | T-Distribution                       | Z-Distribution                      |
|------------------------|--------------------------------------|-------------------------------------|
| Ukuran Sampel          | Kecil (n < 30)                      | Besar (n ≥ 30)                      |
| Simpangan Baku Populasi | Tidak diketahui                      | Diketahui                           |
| Bentuk Distribusi      | Lebih tebal di ekor                  | Kurva normal standar               |
| Penggunaan             | Sampel kecil dan simpangan baku tidak diketahui | Sampel besar dan simpangan baku diketahui |

---

### 📚 Referensi

1. Rumsey, D. (2016). *Statistics for Dummies* (2nd ed.). Wiley.  
2. Walpole, R. E., Myers, R. H., Myers, S. L., & Ye, K. (2012). *Probability and Statistics for Engineers and Scientists* (9th ed.). Pearson.  
3. Laerd Statistics. [T-Distribution Guide](https://statistics.laerd.com/statistical-guides/t-distribution-statistical-guide.php)
