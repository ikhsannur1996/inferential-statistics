# 📏 Confidence Interval (CI) dan Margin of Error (MoE) dalam Uji Hipotesis

---

## 🎯 Apa Itu Confidence Interval?

**Confidence Interval (CI)** atau *interval kepercayaan* adalah **rentang estimasi** yang digunakan untuk menyatakan **sejauh mana kita yakin** bahwa nilai parameter populasi (seperti rata-rata atau proporsi) berada di dalamnya, berdasarkan data dari sampel.

CI selalu disertai dengan **tingkat kepercayaan (confidence level)**, seperti 90%, 95%, atau 99%. Ini adalah ukuran **probabilitas bahwa rentang tersebut mencakup nilai parameter populasi yang sesungguhnya**.

### 🔍 Penjelasan dengan Ilustrasi Konseptual

Jika kita membuat banyak sampel dari populasi dan menghitung CI untuk masing-masing sampel, maka **sekitar 95% dari seluruh CI yang kita buat akan mencakup nilai parameter populasi sebenarnya**, jika tingkat kepercayaan yang digunakan adalah 95%.

> Misalnya, CI 95% dari rata-rata pengeluaran rumah tangga adalah **Rp2.800.000 – Rp3.200.000**. Ini berarti kita 95% yakin bahwa rata-rata pengeluaran populasi seluruh rumah tangga berada dalam rentang tersebut.

---

## 📉 Apa Itu Margin of Error?

**Margin of Error (MoE)** adalah besarnya **batas kesalahan** dari estimasi statistik. MoE menunjukkan **seberapa jauh** nilai hasil sampel mungkin berbeda dari nilai parameter populasi sebenarnya karena **fluktuasi acak** dari pengambilan sampel.

Biasanya ditulis dalam format ± (plus-minus) dan digunakan sebagai komponen utama dalam menghitung Confidence Interval.

> Jika hasil survei menunjukkan 60% orang mendukung kebijakan X, dan MoE adalah ±4%, maka proporsi sebenarnya di populasi diperkirakan antara **56% hingga 64%**.

---

## 🔄 Hubungan Antara Confidence Interval dan Margin of Error

Rumus dasar untuk menghitung **Confidence Interval (CI)**:

```markdown
CI = Estimasi Sampel ± Margin of Error
```

Margin of Error dapat dihitung menggunakan:

```markdown
MoE = Z * (s / √n)
```

- **Z** = nilai dari distribusi normal standar (bergantung pada tingkat kepercayaan)
- **s** = standar deviasi dari sampel
- **n** = ukuran sampel

---

## 🧪 Contoh Perhitungan Confidence Interval dan Margin of Error

Misalkan:

- Rata-rata tinggi badan siswa (estimasi sampel): **165 cm**
- Standar deviasi: **6 cm**
- Ukuran sampel: **36 siswa**
- Tingkat kepercayaan: **95%**
- Nilai Z untuk 95% confidence = **1.96**

### ✍️ Perhitungan:

```markdown
1. Hitung Standard Error (SE):
   SE = s / √n
      = 6 / √36
      = 6 / 6
      = 1

2. Hitung Margin of Error:
   MoE = Z * SE
       = 1.96 * 1
       = 1.96

3. Hitung Confidence Interval:
   CI = Estimasi ± MoE
      = 165 ± 1.96
      = (163.04 cm, 166.96 cm)
```

### ✅ Interpretasi:

> Dengan tingkat kepercayaan 95%, kita yakin bahwa rata-rata tinggi badan seluruh siswa berada dalam rentang **163.04 cm hingga 166.96 cm**.

---

## 📦 Faktor yang Mempengaruhi Confidence Interval dan Margin of Error

| Faktor                        | Pengaruh terhadap CI dan MoE                                         |
|------------------------------|----------------------------------------------------------------------|
| **Ukuran Sampel (n)**        | Semakin besar ukuran sampel, semakin kecil MoE, CI semakin sempit   |
| **Standar Deviasi (s)**      | Semakin tinggi variasi data, semakin besar MoE, CI semakin lebar    |
| **Tingkat Kepercayaan (%)**  | Semakin tinggi confidence level, semakin besar Z, CI makin lebar    |

---

## 🔬 Peran CI dan MoE dalam Uji Hipotesis

Dalam uji hipotesis, kita sering menguji apakah nilai **parameter yang diasumsikan oleh hipotesis nol (H₀)** masuk dalam rentang Confidence Interval.

### 📌 Keputusan:

- **Jika nilai H₀ berada di dalam CI** → **tidak ada cukup bukti** untuk menolak H₀.
- **Jika nilai H₀ berada di luar CI** → kita **menolak H₀**, dan menyimpulkan bahwa perbedaan signifikan.

---

## 🖼️ Ilustrasi CI dan MoE (ASCII)

Misalkan:

- Estimasi rata-rata: 165 cm  
- CI 95%: (163.04 cm, 166.96 cm)

```text
    |---------------|---------------|---------------|
  162             163.04          165           166.96           168
        <------ 95% Confidence Interval -------->
```

Jika hipotesis nol menyatakan rata-rata = 167, maka karena **167 berada di luar CI**, maka kita **menolak H₀**.

---

## 📊 Ringkasan Perbandingan Confidence Interval vs Margin of Error

| Aspek                          | Confidence Interval (CI)                                        | Margin of Error (MoE)                                     |
|-------------------------------|------------------------------------------------------------------|-----------------------------------------------------------|
| **Definisi**                  | Rentang nilai estimasi parameter populasi dengan tingkat keyakinan tertentu. | Batas maksimum kesalahan estimasi terhadap parameter populasi. |
| **Fungsi**                    | Menyatakan rentang di mana nilai sebenarnya kemungkinan besar berada. | Mengukur seberapa besar kemungkinan hasil estimasi menyimpang dari nilai sebenarnya. |
| **Bentuk Hasil**              | Dua angka batas bawah dan atas: *Estimasi ± MoE*               | Satu angka dalam bentuk ± nilai tertentu.                 |
| **Dihitung dari**             | Estimasi sampel dan Margin of Error                             | Z-score, standar deviasi, dan ukuran sampel               |
| **Terkait Tingkat Kepercayaan** | Ya. Semakin tinggi tingkat kepercayaan, semakin lebar interval. | Ya. Semakin tinggi tingkat kepercayaan, semakin besar MoE. |
| **Interpretasi**              | “Kita 95% yakin bahwa nilai sebenarnya berada dalam rentang ini.” | “Hasil bisa meleset sebesar ini dari nilai sebenarnya.”   |
| **Peran dalam Uji Hipotesis** | Digunakan untuk memutuskan apakah hipotesis nol masuk dalam rentang estimasi. | Digunakan sebagai dasar membentuk Confidence Interval.    |

---

## 📚 Referensi

- Rumsey, D. (2016). *Statistics for Dummies*. Wiley.  
- Moore, D. S., McCabe, G. P., & Craig, B. A. (2014). *Introduction to the Practice of Statistics* (8th ed.). W.H. Freeman.  
- Khan Academy. [Confidence Intervals](https://www.khanacademy.org/math/statistics-probability/confidence-intervals-one-sample)
