## 📌 **Bayes' Theorem dalam Uji Hipotesis dengan Contoh Kalkulasi dan Penerapan**

### ⚖️ **Apa Itu Bayes' Theorem?**

**Bayes' Theorem** adalah rumus matematis yang memungkinkan kita untuk **memperbarui probabilitas** suatu hipotesis berdasarkan bukti atau data baru. Dalam uji hipotesis, Bayes' Theorem digunakan untuk **menilai ulang probabilitas** bahwa hipotesis tertentu benar setelah kita memperoleh data atau informasi baru.

Pada dasarnya, Bayes' Theorem menggabungkan **pengetahuan awal** (dikenal sebagai **prior probability**) dengan **bukti baru** (dikenal sebagai **likelihood**) untuk memberikan **probabilitas yang lebih tepat** (dikenal sebagai **posterior probability**).

---

### 🧮 **Rumus Bayes' Theorem**

Secara matematis, **Bayes' Theorem** dapat ditulis sebagai:

![image](https://github.com/user-attachments/assets/8199b807-895c-498b-bb99-136f5d2a2013)

---

### 🔍 **Contoh Penerapan Bayes' Theorem dalam Uji Hipotesis**

Misalkan kita ingin menguji apakah ada perbedaan rata-rata tinggi badan antara pria dan wanita di suatu populasi. Kita mengajukan dua hipotesis:

- **Hipotesis Nol (H₀)**: Tidak ada perbedaan rata-rata tinggi badan antara pria dan wanita.
- **Hipotesis Alternatif (H₁)**: Ada perbedaan rata-rata tinggi badan antara pria dan wanita.

Kita mengumpulkan data dan menghitung nilai p (p-value) berdasarkan data yang ada. Namun, daripada hanya bergantung pada nilai p, kita dapat menggunakan Bayes' Theorem untuk memperbarui probabilitas bahwa H₀ atau H₁ benar, mengingat informasi awal (**prior probability**) dan bukti yang kita peroleh dari data.

#### **Informasi yang Diketahui:**
1. **Prior Probability (P(H))**: Misalnya, berdasarkan pengetahuan sebelumnya, kita tahu bahwa dalam populasi ini, perbedaan rata-rata tinggi badan antara pria dan wanita biasanya kecil. Oleh karena itu, kita memberikan **prior probability yang lebih tinggi** untuk hipotesis nol (H₀).
   - \( P(H₀) = 0,80 \) (80% kemungkinan bahwa tidak ada perbedaan tinggi badan)
   - \( P(H₁) = 0,20 \) (20% kemungkinan bahwa ada perbedaan tinggi badan)

2. **Likelihood (P(D | H))**: Kita juga mengetahui kemungkinan memperoleh data yang ada berdasarkan hipotesis:
   - \( P(D | H₀) = 0,10 \) (10% kemungkinan memperoleh data yang ada jika hipotesis nol benar)
   - \( P(D | H₁) = 0,30 \) (30% kemungkinan memperoleh data yang ada jika hipotesis alternatif benar)

#### **Pertanyaan yang Ingin Dijawab:**
Berdasarkan data yang kita kumpulkan, berapa probabilitas bahwa hipotesis nol (H₀) atau hipotesis alternatif (H₁) lebih mungkin benar?

---

### 🧮 **Langkah-langkah Kalkulasi:**

1. **Hitung \( P(D) \)**, yaitu probabilitas total memperoleh data yang ada (terlepas dari hipotesis yang benar):
![image](https://github.com/user-attachments/assets/cb43d45d-b3d4-4b64-8c38-5ea35c7a5272)


2. **Hitung \( P(H₀ | D) \)**, yaitu probabilitas bahwa hipotesis nol (H₀) benar setelah melihat data:
![image](https://github.com/user-attachments/assets/fc4294ec-e831-4397-921b-6c698de4a656)

3. **Hitung \( P(H₁ | D) \)**, yaitu probabilitas bahwa hipotesis alternatif (H₁) benar setelah melihat data:
![image](https://github.com/user-attachments/assets/fb00c556-4cef-481f-b556-adb235f8f3c2)


---

### 💡 **Interpretasi Hasil:**

Berdasarkan perhitungan Bayes' Theorem, kita mendapatkan:
- **P(H₀ | D) ≈ 0,5714** atau sekitar **57,14%** probabilitas bahwa hipotesis nol (tidak ada perbedaan tinggi badan) benar.
- **P(H₁ | D) ≈ 0,4286** atau sekitar **42,86%** probabilitas bahwa hipotesis alternatif (ada perbedaan tinggi badan) benar.

Meskipun data yang diperoleh menunjukkan ada kemungkinan perbedaan, probabilitas bahwa hipotesis nol masih lebih tinggi (57,14%) dibandingkan dengan hipotesis alternatif (42,86%) karena **prior probability** bahwa tidak ada perbedaan lebih besar.

---

### 🧠 **Keunggulan Bayes' Theorem dalam Uji Hipotesis**

1. **Mengintegrasikan Pengetahuan Sebelumnya**: Salah satu keunggulan utama menggunakan Bayes' Theorem adalah kemampuannya untuk menggabungkan **pengetahuan sebelumnya** (prior) dengan **data baru**. Hal ini memungkinkan kita untuk membuat keputusan yang lebih informasional dan tidak hanya bergantung pada hasil pengujian yang terisolasi.

2. **Probabilitas Berubah Seiring Waktu**: Bayes' Theorem memberikan cara untuk **memperbarui probabilitas** seiring dengan bertambahnya data. Ini sangat berguna dalam situasi di mana data baru diperoleh secara bertahap, dan kita perlu memperbarui keputusan kita dengan informasi yang lebih baik.

3. **Penyajian Informasi Lebih Lengkap**: Dengan menggunakan Bayes' Theorem, kita dapat memperoleh **probabilitas terperinci** mengenai apakah hipotesis kita benar atau tidak, alih-alih hanya mengandalkan keputusan "menolak atau gagal menolak hipotesis nol" berdasarkan nilai p.

---

### ⚖️ **Perbedaan Pendekatan Frequentist dan Bayesian dalam Uji Hipotesis**

| **Aspek**                | **Pendekatan Frequentist (p-value)**                              | **Pendekatan Bayesian (Bayes' Theorem)**                                 |
|--------------------------|-------------------------------------------------------------------|------------------------------------------------------------------------|
| **Fokus**                 | Menggunakan data untuk menguji apakah hasil tersebut mungkin terjadi jika hipotesis nol benar | Memperbarui probabilitas suatu hipotesis berdasarkan data dan pengetahuan sebelumnya |
| **Keputusan**             | Menolak atau gagal menolak hipotesis nol berdasarkan nilai p     | Menghitung probabilitas bahwa hipotesis benar setelah data dikumpulkan |
| **Pengetahuan Awal (Prior)** | Tidak menggunakan prior, hanya berdasarkan data yang ada       | Menggunakan prior probability untuk memperbarui keputusan setelah mendapatkan data |
| **Hasil**                 | Keputusan akhir berupa "menolak" atau "gagal menolak" hipotesis  | Probabilitas terperinci tentang kebenaran hipotesis berdasarkan data dan prior |

---

### 📚 **Referensi**

1. Rumsey, D. (2016). *Statistics for Dummies* (2nd ed.). Wiley.
2. Walpole, R. E., Myers, R. H., Myers, S. L., & Ye, K. (2012). *Probability and Statistics for Engineers and Scientists* (9th ed.). Pearson.
3. Laerd Statistics. [Bayes' Theorem](https://statistics.laerd.com/statistical-guides/bayes-theorem-statistical-guide.php).
4. Gelman, A., Carlin, J. B., Stern, H. S., Dunson, D. B., Vehtari, A., & Rubin, D. B. (2014). *Bayesian Data Analysis* (3rd ed.). CRC Press.
