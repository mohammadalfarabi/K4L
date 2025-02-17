---
title: SISTEM PERSAMAAN LINIER

---

# SISTEM PERSAMAAN LINIER

## Definisi Sistem Persamaan Linier
Sistem persamaan linier adalah kumpulan dari satu atau lebih persamaan linier yang memiliki variabel yang sama. Bentuk umum dari sistem persamaan linier dengan n variabel adalah:

$a_1x_1 + a_2x_2 + \dots + a_nx_n = b$

Di mana:
- $( a_1, a_2, ..., a_n )$ adalah koefisien,
- $( x_1, x_2, ..., x_n )$ adalah variabel,
- $( b )$ adalah konstanta.

Sistem persamaan linier dapat memiliki solusi unik, banyak solusi, atau tidak memiliki solusi tergantung pada sifat dari persamaan dalam sistem tersebut.

## Solusi Persamaan Linier
Solusi dari sistem persamaan linier dapat ditemukan dengan berbagai metode, di antaranya:

### Eliminasi
Metode eliminasi adalah teknik penyelesaian sistem persamaan linier dengan menghilangkan variabel secara bertahap hingga memperoleh bentuk yang lebih sederhana. Langkah-langkah metode eliminasi adalah:
1. Pilih satu variabel untuk dieliminasi.
2. Kalikan salah satu atau kedua persamaan sehingga koefisien variabel yang ingin dieliminasi menjadi sama.
3. Kurangkan atau tambahkan persamaan untuk menghilangkan variabel tersebut.
4. Ulangi langkah di atas hingga sistem menjadi lebih sederhana dan mudah diselesaikan.

**Contoh:**

$\begin{cases}
y = 2x + 3 \\
x + y = 15
\end{cases}$
 
Langkah-langkah:  
1. Substitusi $y = 2x + 3$ ke persamaan kedua:

   $x + (2x + 3) = 15$

2. Sederhanakan:

   $x + 2x + 3 = 15$

   $3x + 3 = 15$

   $3x = 12$

   $x = 4$

3. Substitusi $x = 4$ ke $y = 2x + 3$:

   $y = 2(4) + 3 = 8 + 3 = 11$

**Solusi: $(4,11)$**

### Eliminasi Gauss
Eliminasi Gauss adalah metode yang digunakan untuk menyederhanakan sistem persamaan linier ke dalam bentuk eselon baris. Langkah-langkahnya adalah:
1. Susun sistem persamaan dalam bentuk matriks augmented.
2. Gunakan operasi baris elementer untuk mengubah matriks ke bentuk eselon baris.
3. Dari bentuk eselon baris, gunakan substitusi balik untuk menemukan nilai variabel.

**Contoh:**

$\begin{bmatrix} 
1 & -2 & | -3 \\ 
1 & 1 & | 15 
\end{bmatrix}$

1. Eliminasi elemen pertama dari baris kedua dengan $R_2 \leftarrow R_2 - R_1$:

   $\begin{bmatrix} 
   1 & -2 & | -3 \\ 
   0 & 3 & | 18 
   \end{bmatrix}$
   
2. Bagi baris kedua dengan 3 agar $y$ menjadi 1:
   
   $\begin{bmatrix} 
   1 & -2 & | -3 \\ 
   0 & 1 & | 6 
   \end{bmatrix}$
   
3. Gunakan $R_1 \leftarrow R_1 + 2R_2$ untuk menghilangkan elemen kedua di baris pertama:
   
   $\begin{bmatrix} 
   1 & 0 & | 4 \\ 
   0 & 1 & | 6 
   \end{bmatrix}$
   

Sehingga diperoleh **$x = 4$ dan $y = 11$**.

### Solusi Grafik
Metode solusi grafik digunakan untuk sistem persamaan linier dengan dua variabel. Langkah-langkahnya adalah:
1. Gambarkan masing-masing persamaan sebagai garis pada bidang koordinat.
2. Titik potong antara dua garis tersebut adalah solusi dari sistem.
3. Jika garis berpotongan di satu titik, maka ada satu solusi unik.
4. Jika garis sejajar, maka tidak ada solusi.
5. Jika garis bertumpuk, maka ada banyak solusi.

**Contoh:**
Untuk sistem persamaan:

$\begin{cases}
y = 2x + 3\\
y = -x + 15
\end{cases}$

<iframe src="https://www.geogebra.org/calculator/nsjfzexc?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>


