## 📌 Apa Itu *p-value* dalam Uji Hipotesis?

### 🧠 Pengertian Umum

**p-value** atau **nilai probabilitas** adalah suatu ukuran statistik yang digunakan untuk membantu menentukan apakah hasil dari suatu uji hipotesis **cukup kuat secara statistik** untuk menolak hipotesis nol (**H₀**).

Secara sederhana, **p-value menunjukkan seberapa besar kemungkinan kita mendapatkan hasil seperti yang diamati (atau lebih ekstrem)**, **jika hipotesis nol (H₀) benar**.

---

### 🔍 Penjelasan dalam Bahasa Sederhana

Misalnya:
> Anda ingin menguji apakah suatu obat baru lebih efektif dibandingkan obat lama.  
> Anda mengasumsikan awalnya (H₀) bahwa **tidak ada perbedaan efektivitas** antara keduanya.

Setelah dilakukan uji statistik dan diperoleh p-value = **0.02**. Artinya:
- Jika memang tidak ada perbedaan (H₀ benar), maka kemungkinan Anda akan memperoleh hasil seperti itu **hanya sebesar 2% saja**.
- Karena 2% itu **kecil**, maka hasil tersebut **cukup jarang terjadi secara kebetulan**, sehingga Anda bisa **menolak H₀** dan menyimpulkan bahwa kemungkinan besar **ada perbedaan**.

---

### 📐 Interpretasi Nilai p-value

| p-value         | Interpretasi                                                           |
|------------------|------------------------------------------------------------------------|
| **p < 0.01**     | Hasil sangat signifikan; sangat kuat untuk menolak H₀                 |
| **0.01 ≤ p < 0.05** | Hasil signifikan; cukup kuat untuk menolak H₀                        |
| **0.05 ≤ p < 0.10** | Hasil lemah; ada indikasi, tetapi kurang kuat untuk menolak H₀       |
| **p ≥ 0.10**     | Tidak signifikan; tidak ada cukup bukti untuk menolak H₀              |

> **Catatan**: Ambang batas yang umum digunakan adalah **α = 0.05 (5%)**. Artinya, jika **p-value < 0.05**, maka kita **menolak H₀**.

---

### 🖼 Ilustrasi Konsep p-value (Distribusi Normal)

Distribusi normal berikut menunjukkan **nilai uji statistik (z atau t)** dan area yang menunjukkan **p-value**:

```
Distribusi Normal (Two-Tailed Test)

            Wilayah p-value
       <-------------------------->
           |                    |
           |                    |
           |     .       .      |
           |    .         .     |
           |   .           .    |
-----------|--.-----|------.----|-----------
         -zα/2       μ      +zα/2
                    |
                Nilai rata-rata
```

Keterangan:
- Titik-titik di sisi kiri dan kanan menunjukkan hasil yang sangat berbeda dari mean (μ).
- Area di bawah kurva pada kedua sisi ujung (warna gelap dalam ilustrasi visual) adalah **p-value**.
- Semakin kecil p-value, semakin jauh nilai uji dari pusat distribusi, dan semakin kuat alasan menolak H₀.

---

### ⚠️ Hal yang Perlu Diingat

1. **p-value bukan probabilitas bahwa H₀ benar**.  
   Banyak orang salah mengartikan p-value sebagai "kemungkinan H₀ benar", padahal itu tidak tepat secara statistik.

2. **p-value hanya bergantung pada data sampel**.  
   Ia tidak bisa berdiri sendiri tanpa konteks, dan harus dibaca bersamaan dengan ukuran sampel, efek praktis (effect size), dan desain penelitian.

3. **p-value kecil ≠ hasil penting secara praktis**.  
   Bisa jadi perbedaan itu memang signifikan secara statistik, tetapi tidak relevan secara nyata (contoh: selisih suhu 0.2 derajat).

---

### 🧾 Contoh Kasus Sederhana

**Kasus**: Seorang peneliti ingin mengetahui apakah rata-rata waktu tidur mahasiswa kurang dari 7 jam per malam.

- Hipotesis nol: H₀: μ = 7 jam  
- Hipotesis alternatif: H₁: μ < 7 jam

Setelah melakukan uji statistik pada sampel 40 mahasiswa, diperoleh:
- Nilai p = **0.03**

**Interpretasi**:
- Karena **0.03 < 0.05**, maka H₀ ditolak.
- Artinya, terdapat **bukti yang cukup** bahwa rata-rata waktu tidur mahasiswa **kurang dari 7 jam per malam**.

---

### 📚 Referensi

1. Rumsey, D. (2016). *Statistics for Dummies* (2nd ed.). Wiley.  
2. Motulsky, H. (2014). *Intuitive Biostatistics* (3rd ed.). Oxford University Press.  
3. Laerd Statistics. [Understanding p-values](https://statistics.laerd.com/statistical-guides/understanding-p-values-statistical-guide.php)  
4. NIST/SEMATECH e-Handbook of Statistical Methods. [What is a p-value?](https://www.itl.nist.gov/div898/handbook/prc/section1/prc16.htm)
