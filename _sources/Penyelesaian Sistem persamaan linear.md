---
title: Penyelesaian Sistem persamaan linear

---

# Penyelesaian Sistem persamaan linear
## Operasi Baris Elementer
### Elemenasi Gauss


#### 1. Soal nomor 1

$\begin{aligned}
\quad x_1 + 2x_2 + 3x_3 &= 6 \\
\quad 2x_1 + 4x_2 + 6x_3 &= 12 \\
\quad x_2 + x_3 &= 2
\end{aligned}$

**Langkah 1: Representasi Matriks Augmented**
Kita ubah sistem persamaan ini menjadi bentuk matriks augmented:

$\begin{bmatrix}
1 & 2 & 3 & | 6 \\
2 & 4 & 6 & | 12 \\
0 & 1 & 1 & | 2
\end{bmatrix}$

**Langkah 2: Eliminasi Baris**
**Eliminasi Elemen di Kolom Pertama**
- Kita ingin membuat elemen di bawah elemen utama (pivot) pertama menjadi nol.
- Baris kedua dikurangi 2 kali baris pertama:  

$4R_2 = R_2 - 2R_1$

$\begin{bmatrix}
1 & 2 & 3 & | 6 \\
0 & 0 & 0 & | 0 \\
0 & 1 & 1 & | 2
\end{bmatrix}$

Karena baris kedua menjadi nol sepenuhnya, ini menunjukkan bahwa **baris tersebut tidak memberikan informasi tambahan**, sehingga kita bisa mengabaikannya.

**Langkah 3: Ubah ke Bentuk Eselon Baris**
Matriks yang tersisa:

$\begin{bmatrix}
1 & 2 & 3 & | 6 \\
0 & 1 & 1 & | 2
\end{bmatrix}$

Kita sudah memiliki bentuk eselon baris.

 **Langkah 4: Substitusi Balik**
Dari baris kedua:

$x_2 + x_3 = 2$

$x_2 = 2 - x_3$

Dari baris pertama:

$x_1 + 2x_2 + 3x_3 = 6$

Substitusi $( x_2 = 2 - x_3 )$:

$x_1 + 2(2 - x_3) + 3x_3 = 6$

$x_1 + 4 - 2x_3 + 3x_3 = 6$

$x_1 + 4 + x_3 = 6$

$x_1 = 2 - x_3$

**Hasil Akhir**
Solusi dalam bentuk parametrik:

$\begin{aligned}
x_1 &= 2 - x_3 \\
x_2 &= 2 - x_3 \\
x_3 &= x_3
\end{aligned}$

Karena ada satu variabel bebas $( x_3 )$, maka sistem ini memiliki **tak hingga banyak solusi**. 

Jika ingin solusi spesifik, kita bisa memilih nilai $( x_3 )$, misalnya:
- Jika $( x_3 = 0 )$ → $( (x_1, x_2, x_3) = (2,2,0) )$.
- Jika $( x_3 = 1 )$ → $( (x_1, x_2, x_3) = (1,1,1) )$.
- Jika $( x_3 = 2 )$ → $( (x_1, x_2, x_3) = (0,0,2) )$.

---

#### 2. Soal nomor 2

$\begin{aligned}
\quad x_1 + x_2 + x_3 &= 3 \\
\quad 2x_1 + 2x_3 &= 5 \\
\quad x_1 + 2x_2 &= 3
\end{aligned}$

**Langkah 1: Representasi Matriks Augmented**
Kita ubah sistem persamaan ke dalam bentuk matriks augmented:

$\begin{bmatrix}
1 & 1 & 1 & | 3 \\
2 & 0 & 2 & | 5 \\
1 & 2 & 0 & | 3
\end{bmatrix}$

**Langkah 2: Eliminasi Elemen di Bawah Pivot Pertama**
Kita buat elemen di bawah elemen utama (pivot) pertama menjadi nol dengan operasi baris:

- $( R_2 = R_2 - 2R_1 )$
- $( R_3 = R_3 - R_1 )$

$\begin{bmatrix}
1 & 1 & 1 & | 3 \\
0 & -2 & 0 & | -1 \\
0 & 1 & -1 & | 0
\end{bmatrix}$

**Langkah 3: Eliminasi Elemen di Bawah Pivot Kedua**
Sekarang kita eliminasi elemen di bawah pivot kedua ($( -2 )$) untuk mendapatkan bentuk eselon:

- $( R_3 = R_3 + \frac{1}{2} R_2 )$


$\begin{bmatrix}
1 & 1 & 1 & | 3 \\
0 & -2 & 0 & | -1 \\
0 & 0 & -1 & | -\frac{1}{2}
\end{bmatrix}$

**Langkah 4: Substitusi Balik**
Dari baris ketiga:

$- x_3 = -\frac{1}{2}$

$x_3 = \frac{1}{2}$

Dari baris kedua:

$-2x_2 = -1$

$x_2 = \frac{1}{2}$

Dari baris pertama:

$x_1 + x_2 + x_3 = 3$

$x_1 + \frac{1}{2} + \frac{1}{2} = 3$

$x_1 + 1 = 3$

$x_1 = 2$

**Hasil Akhir**
Solusi unik dari sistem ini adalah:

$(x_1, x_2, x_3) = (2, \frac{1}{2}, \frac{1}{2})$

Jadi, sistem ini memiliki **solusi tunggal** yaitu **$( x_1 = 2 \), \( x_2 = \frac{1}{2} \), \( x_3 = \frac{1}{2} )$**. 

---

#### 3. Soal nomor 3
$2x_1 + 2x_2 = 4$
$x_1 + x_1 = 2$

**Langkah 1: Representasi Matriks Augmented**
Kita ubah sistem persamaan ini menjadi bentuk matriks augmented:


$\begin{bmatrix}
2 & 2 & | 4 \\
1 & 1 & | 2
\end{bmatrix}$

**Langkah 2: Normalisasi Pivot (Bentuk Eselon Baris)**
Kita buat elemen pivot pertama menjadi 1 dengan membagi baris pertama dengan 2:

$R_1 = \frac{1}{2} R_1$

$\begin{bmatrix}
1 & 1 & | 2 \\
1 & 1 & | 2
\end{bmatrix}$

Selanjutnya, kita eliminasi elemen di bawah pivot dengan $( R_2 = R_2 - R_1 )$:

$\begin{bmatrix}
1 & 1 & | 2 \\
0 & 0 & | 0
\end{bmatrix}$

**Langkah 3: Substitusi Balik**
Dari baris pertama:

$x_1 + x_2 = 2$

Dari baris kedua, kita lihat bahwa $( 0 = 0 )$, yang selalu benar, sehingga baris ini tidak memberikan informasi tambahan.

Maka, sistem memiliki **tak hingga banyak solusi**, tergantung pada nilai variabel bebas $( x_2 )$:

$\begin{aligned}
x_1 &= 2 - x_2 \\
x_2 &= x_2
\end{aligned}$

 **Hasil Akhir**
Solusi dalam bentuk parametrik:

$(x_1, x_2) = (2 - x_2, x_2)$

Misalnya:
- Jika $( x_2 = 0 )$, maka $( (x_1, x_2) = (2, 0) )$.
- Jika $( x_2 = 1 )$, maka $( (x_1, x_2) = (1, 1) )$.
- Jika $( x_2 = 2 )$, maka $( (x_1, x_2) = (0, 2) )$.

Sistem ini memiliki **tak hingga banyak solusi** karena kedua persamaan sebenarnya identik.

---

#### 4. Soal nomor 4

$\begin{aligned}
\quad x_1 + x_2 &= 5 \\
\quad x_1 + 2x_2 &= 6
\end{aligned}$

**Langkah 1: Representasi Matriks Augmented**
Kita ubah sistem persamaan menjadi bentuk matriks augmented:

$\begin{bmatrix}
1 & 1 & | 5 \\
1 & 2 & | 6
\end{bmatrix}$

**Langkah 2: Eliminasi Baris**
Kita eliminasi elemen di bawah pivot pertama. Caranya, kurangkan baris kedua dengan baris pertama:

$R_2 = R_2 - R_1$

$\begin{bmatrix}
1 & 1 & | 5 \\
0 & 1 & | 1
\end{bmatrix}$

**Langkah 3: Substitusi Balik**
Dari baris kedua:

$x_2 = 1$

Substitusi $( x_2 = 1 )$ ke dalam baris pertama:

$x_1 + 1 = 5$

$x_1 = 4$

**Hasil Akhir**
Solusi unik:

$(x_1, x_2) = (4, 1)$

Jadi, sistem ini memiliki **solusi tunggal** yaitu **$( x_1 = 4 )$, $( x_2 = 1 )$**.

