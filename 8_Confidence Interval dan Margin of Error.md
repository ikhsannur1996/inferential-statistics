## 📏 **Confidence Interval (CI) dan Margin of Error (MoE) dalam Uji Hipotesis**

---

### 🎯 1. **Apa Itu Confidence Interval (CI)?**

**Confidence Interval** atau **interval kepercayaan** adalah rentang nilai yang digunakan untuk memperkirakan **parameter populasi** (seperti rata-rata atau proporsi), berdasarkan informasi dari **sampel**.

Rentang ini disusun agar memiliki tingkat keyakinan tertentu, seperti **90%**, **95%**, atau **99%**, yang menyatakan seberapa **yakin** kita bahwa nilai sebenarnya dari populasi berada dalam rentang tersebut.

#### ✔️ Contoh:
Jika hasil survei menunjukkan bahwa rata-rata pengeluaran bulanan responden adalah **Rp3.000.000**, dan interval kepercayaan 95% adalah:

\[
CI = Rp2.800.000 \text{ s/d } Rp3.200.000
\]

Artinya, **kita 95% yakin** bahwa rata-rata pengeluaran bulanan seluruh populasi (bukan hanya sampel) berada dalam rentang tersebut.

---

### 📉 2. **Apa Itu Margin of Error (MoE)?**

**Margin of Error** adalah batas maksimum penyimpangan hasil estimasi dari sampel terhadap nilai sebenarnya pada populasi. MoE menunjukkan **seberapa besar ketidakpastian** dari estimasi tersebut.

Biasanya ditulis dalam bentuk plus-minus (±) dan merupakan salah satu komponen pembentuk confidence interval.

#### ✔️ Contoh:
Jika survei mengatakan bahwa **60% orang memilih opsi A**, dan **MoE = ±4%**, maka hasil sebenarnya di populasi mungkin berada antara:

\[
60\% - 4\% = 56\%, \quad \text{dan} \quad 60\% + 4\% = 64\%
\]

---

### 🔄 3. **Hubungan Confidence Interval dan Margin of Error**

Secara matematis, interval kepercayaan dibentuk dari:

\[
\text{Confidence Interval} = \text{Estimasi Sampel} \pm \text{Margin of Error}
\]

Margin of Error tergantung pada:
- **Tingkat kepercayaan (confidence level)**: Semakin tinggi tingkat kepercayaan (misal 99%), maka MoE dan CI menjadi lebih **lebar**.
- **Ukuran sampel**: Semakin banyak data (sampel besar), maka MoE menjadi lebih **kecil** dan CI lebih **sempit**.
- **Variabilitas data (standar deviasi)**: Semakin beragam datanya, semakin besar MoE-nya.

---

### 🧪 4. **Peran CI dan MoE dalam Uji Hipotesis**

Dalam uji hipotesis, kita membandingkan nilai hipotesis (biasanya dari **H₀**) dengan **confidence interval** dari hasil sampel.

- Jika **nilai hipotesis (H₀)** berada **di dalam CI**, maka **tidak cukup bukti** untuk menolak H₀.
- Jika **nilai hipotesis berada di luar CI**, maka kita bisa **menolak H₀**, artinya hasilnya **signifikan secara statistik**.

---

### 💡 5. **Visualisasi Sederhana (Ilustrasi ASCII)**

Misalnya kita punya hasil estimasi:
- Rata-rata tinggi = 165 cm
- MoE = ±3 cm
- CI (95%) = 162 cm sampai 168 cm

Berikut ilustrasinya:

```
|---------------------|-------------------------|---------------------|
159 cm              162 cm                  165 cm              168 cm              171 cm
      [---------- Confidence Interval (95%) -----------]
```

Jika nilai hipotesis nol (misalnya H₀: rata-rata = 170 cm) **berada di luar CI**, maka H₀ dapat **ditolak**.

---

### 📦 6. **Ringkasan Perbandingan**

| Aspek                      | Confidence Interval (CI)                             | Margin of Error (MoE)                         |
|----------------------------|-----------------------------------------------------|------------------------------------------------|
| Fungsi                    | Menunjukkan rentang estimasi parameter populasi     | Menyatakan seberapa besar kemungkinan kesalahan |
| Bentuk                    | Rentang: estimasi ± MoE                             | Nilai tunggal: selisih estimasi ke batas CI   |
| Digunakan untuk           | Menilai akurasi estimasi dan menguji hipotesis      | Menjelaskan tingkat ketidakpastian hasil      |
| Tergantung pada           | Sampel, variansi, dan tingkat kepercayaan           | Sampel, variansi, tingkat kepercayaan         |

---

### 📚 **Referensi**:
1. Rumsey, D. (2016). *Statistics for Dummies*. Wiley.  
2. Moore, D. S., McCabe, G. P., & Craig, B. A. (2014). *Introduction to the Practice of Statistics*. W.H. Freeman.  
3. Khan Academy. [Confidence Intervals](https://www.khanacademy.org/math/statistics-probability/confidence-intervals-one-sample)

---
