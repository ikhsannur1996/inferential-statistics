## 📌 Apa Itu Z-Test dalam Uji Hipotesis?

### 🧠 Pengertian Umum

**Z-test** adalah salah satu jenis uji statistik yang digunakan dalam **uji hipotesis** untuk menentukan apakah terdapat **perbedaan yang signifikan** antara **rata-rata sampel** dan **rata-rata populasi**, atau antara **dua rata-rata sampel**, **dengan asumsi bahwa data berdistribusi normal** dan **simpangan baku (standar deviasi) populasi diketahui**.

---

### 🧪 Kapan Z-Test Digunakan?

Z-test umumnya digunakan ketika:
1. Ukuran sampel cukup besar (**n ≥ 30**).
2. Data mengikuti distribusi normal (atau mendekatinya karena ukuran sampel besar).
3. **Simpangan baku populasi (σ)** diketahui.
4. Pengujian melibatkan **rata-rata (mean)**.

---

### 📐 Rumus Z-Test

Untuk satu sampel, rumus Z-test adalah:

![image](https://github.com/user-attachments/assets/566bd256-9fe9-4981-ad96-1e25941853ad)


---

### 🔍 Penjelasan Sederhana

Bayangkan Anda adalah seorang kepala sekolah yang ingin mengetahui apakah rata-rata nilai matematika siswa tahun ini berbeda dari nilai rata-rata tahun lalu yang diketahui adalah **75**.

1. Anda ambil sampel 40 siswa dari tahun ini.
2. Nilai rata-rata sampel adalah 78.
3. Anda tahu dari tahun-tahun sebelumnya bahwa simpangan baku populasi adalah 10.
4. Anda ingin tahu: Apakah perbedaan nilai itu **kebetulan saja** atau memang **berarti secara statistik**?

Dengan menggunakan rumus Z-test, Anda bisa menghitung nilai **Z-score**, lalu dibandingkan dengan **nilai kritis Z** berdasarkan tingkat signifikansi yang Anda tentukan (misalnya α = 0.05).

---

### 📊 Interpretasi Hasil Z-Test

Setelah nilai Z dihitung, interpretasinya sebagai berikut:

- Jika nilai **Z berada di luar wilayah kritis**, maka:
  - **Tolak H₀** → Ada cukup bukti bahwa rata-rata berbeda.
- Jika nilai **Z berada dalam wilayah netral**, maka:
  - **Gagal menolak H₀** → Tidak cukup bukti untuk menyatakan bahwa rata-rata berbeda.

Contoh:
- Z-hitung = 2.5  
- Z-kritis untuk α = 0.05 (two-tailed) = ±1.96  
- Karena 2.5 > 1.96 → Tolak H₀ → Perbedaan signifikan

---

### 🧾 Contoh Kasus Sederhana

**Masalah**: Seorang peneliti ingin mengetahui apakah minuman energi baru meningkatkan rata-rata waktu lari atlet.

- Rata-rata waktu populasi: 15 menit
- Sampel 36 atlet, rata-rata waktu: 14.5 menit
- Simpangan baku populasi: 1.8 menit
- α = 0.05

**Langkah-langkah**:
1. Rumus Z:  
![image](https://github.com/user-attachments/assets/d2b899c6-1ef7-4901-b830-94a629c4ca6a)

2. Z-kritis untuk uji dua sisi (α = 0.05) = ±1.96  
3. Karena -1.67 berada dalam wilayah netral → **Gagal menolak H₀**

**Kesimpulan**: Tidak cukup bukti bahwa minuman tersebut meningkatkan waktu lari secara signifikan.

---

### 🧠 Perbedaan Z-Test dan T-Test

| Aspek               | Z-Test                         | T-Test                          |
|---------------------|--------------------------------|----------------------------------|
| Ukuran sampel       | Umumnya ≥ 30                   | Umumnya < 30                    |
| Diketahui σ         | Ya                             | Tidak diketahui (gunakan s)     |
| Distribusi          | Normal                         | Normal (atau mendekati)         |

---

### 🖼 Ilustrasi Z-Test dalam Diagram ASCII

Distribusi Normal (Z-Test)

```
        Wilayah Tolak H₀ (p-value)                  Wilayah Tolak H₀ (p-value)
       <------------------------------|----------------------------------->
                -Z(α/2)                 |               +Z(α/2)
                                         |
                          Nilai Rata-rata (μ) 
                                         |
               Wilayah Terima H₀ (Fail to Reject H₀)
                       (Tidak ada cukup bukti)
```

### Penjelasan Ilustrasi:
- **μ** (rata-rata populasi) berada di tengah distribusi normal.
- **Z(α/2)** adalah nilai kritis Z untuk **uji dua sisi** (misalnya **α = 0.05**, maka **α/2 = 0.025** pada setiap sisi).
- **Wilayah Tolak H₀** berada di kedua sisi distribusi normal (area di luar Z(α/2)).
- Jika nilai Z-hitung **terletak di luar wilayah penolakan H₀**, kita **menolak hipotesis nol (H₀)**.
- Jika nilai Z-hitung **terletak di dalam wilayah terima H₀**, kita **gagal menolak hipotesis nol (H₀)**.

---

### 📚 Referensi

1. Rumsey, D. (2016). *Statistics for Dummies* (2nd ed.). Wiley.  
2. Walpole, R. E., Myers, R. H., Myers, S. L., & Ye, K. (2012). *Probability and Statistics for Engineers and Scientists* (9th ed.). Pearson.  
3. Laerd Statistics. [Z-Test Guide](https://statistics.laerd.com/statistical-guides/z-test-statistical-guide.php)
