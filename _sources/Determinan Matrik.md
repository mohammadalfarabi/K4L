---
title: Determinan Matrik

---

# DETERMINAN MATRIKS
Determinant atau determinan matriks adalah suatu bilangan skalar yang diperoleh dari operasi tertentu pada elemen-elemen suatu matriks persegi. Determinan memiliki peran penting dalam berbagai aplikasi matematika, termasuk mencari invers matriks dan menyelesaikan sistem persamaan linear.

## 1. Minor Matriks
Minor dari suatu elemen dalam matriks adalah determinan dari submatriks yang diperoleh dengan menghapus baris dan kolom yang mengandung elemen tersebut.

## 2. Cofaktor Matriks
Cofaktor dari suatu elemen dalam matriks adalah minor dari elemen tersebut dikalikan dengan faktor tanda (-1)ⁱ⁺ʲ, di mana $( i )$ adalah indeks baris dan $( j )$ adalah indeks kolom.

## **3. Mencari Determinan dengan Konsep Minor dan Cofaktor**  
Determinannya dihitung dengan ekspansi kofaktor menggunakan rumus:  
$\det(A) = \sum_{j=1}^{n} a_{ij} C_{ij}$
di mana $( a_{ij} )$ adalah elemen pada baris pertama dan $( C_{ij} )$ adalah kofaktor dari elemen tersebut.


### Contoh Perhitungan Determinan

### 1. Contoh Determinan Matriks 3×3
Misalkan diberikan matriks:  
$A =
\begin{bmatrix}
2 & 3 & 1 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}$
Kita gunakan ekspansi kofaktor pada baris pertama:  
$\det(A) = 2
\begin{vmatrix}
5 & 6 \\
8 & 9
\end{vmatrix} - 3
\begin{vmatrix}
4 & 6 \\
7 & 9
\end{vmatrix} + 1
\begin{vmatrix}
4 & 5 \\
7 & 8
\end{vmatrix}$

Hitung determinan dari masing-masing submatriks 2×2:  
$\begin{vmatrix}
5 & 6 \\
8 & 9
\end{vmatrix} = (5 \times 9) - (6 \times 8) = 45 - 48 = -3$

$\begin{vmatrix}
4 & 6 \\
7 & 9
\end{vmatrix} = (4 \times 9) - (6 \times 7) = 36 - 42 = -6$

$\begin{vmatrix}
4 & 5 \\
7 & 8
\end{vmatrix} = (4 \times 8) - (5 \times 7) = 32 - 35 = -3$

Substitusi hasilnya:  
$\det(A) = (2 \times -3) - (3 \times -6) + (1 \times -3)$
$= -6 + 18 - 3 = 9$

### **2. Contoh Determinan Matriks 4×4**  
Misalkan diberikan matriks:  
$B =
\begin{bmatrix}
1 & 2 & 3 & 4 \\
5 & 6 & 7 & 8 \\
9 & 10 & 11 & 12 \\
13 & 14 & 15 & 16
\end{bmatrix}$
Gunakan ekspansi kofaktor pada baris pertama:  
$\det(B) = 1
\begin{vmatrix}
6 & 7 & 8 \\
10 & 11 & 12 \\
14 & 15 & 16
\end{vmatrix} - 2
\begin{vmatrix}
5 & 7 & 8 \\
9 & 11 & 12 \\
13 & 15 & 16
\end{vmatrix} + 3
\begin{vmatrix}
5 & 6 & 8 \\
9 & 10 & 12 \\
13 & 14 & 16
\end{vmatrix} - 4
\begin{vmatrix}
5 & 6 & 7 \\
9 & 10 & 11 \\
13 & 14 & 15
\end{vmatrix}$

Setiap submatriks 3×3 dihitung dengan metode sebelumnya:  
$\begin{vmatrix}
6 & 7 & 8 \\
10 & 11 & 12 \\
14 & 15 & 16
\end{vmatrix} = (6(11 \times 16 - 12 \times 15)) - (7(10 \times 16 - 12 \times 14)) + (8(10 \times 15 - 11 \times 14))$

$= (6(176 - 180)) - (7(160 - 168)) + (8(150 - 154))$
$= (6 \times -4) - (7 \times -8) + (8 \times -4)$
$= -24 + 56 - 32 = 0$

Karena semua submatriks 3×3 dari ekspansi kofaktor juga bernilai 0, maka:
$\det(B) = 0$


### 3. Contoh Determinan Matriks 5×5
Misalkan diberikan matriks:
$C =
\begin{bmatrix}
1 & 2 & 3 & 4 & 5 \\
6 & 7 & 8 & 9 & 10 \\
11 & 12 & 13 & 14 & 15 \\
16 & 17 & 18 & 19 & 20 \\
21 & 22 & 23 & 24 & 25
\end{bmatrix}$

Gunakan ekspansi kofaktor pada baris pertama:

$\det(C) =
1 \times C_{11} - 2 \times C_{12} + 3 \times C_{13} - 4 \times C_{14} + 5 \times C_{15}$

di mana $( C_{ij} )$ adalah determinan dari submatriks 4×4 yang diperoleh dengan menghapus baris ke-1 dan kolom ke- $( j )$.
Hitung Submatriks 4×4
Misalkan kita hitung submatriks pertama $( C_{11} )$ dengan menghapus baris pertama dan kolom pertama:

$C_{11} =
\begin{vmatrix}
7 & 8 & 9 & 10 \\
12 & 13 & 14 & 15 \\
17 & 18 & 19 & 20 \\
22 & 23 & 24 & 25
\end{vmatrix}$

Gunakan ekspansi kofaktor pada baris pertama dari $( C_{11} )$:
$\begin{vmatrix}
7 & 8 & 9 & 10 \\
12 & 13 & 14 & 15 \\
17 & 18 & 19 & 20 \\
22 & 23 & 24 & 25
\end{vmatrix} = 7
\begin{vmatrix}
13 & 14 & 15 \\
18 & 19 & 20 \\
23 & 24 & 25
\end{vmatrix} - 8
\begin{vmatrix}
12 & 14 & 15 \\
17 & 19 & 20 \\
22 & 24 & 25
\end{vmatrix} + 9
\begin{vmatrix}
12 & 13 & 15 \\
17 & 18 & 20 \\
22 & 23 & 25
\end{vmatrix} - 10
\begin{vmatrix}
12 & 13 & 14 \\
17 & 18 & 19 \\
22 & 23 & 24
\end{vmatrix}$

Hitung Submatriks 3×3
Misalkan kita hitung determinan submatriks 3×3 pertama:

$\begin{vmatrix}
13 & 14 & 15 \\
18 & 19 & 20 \\
23 & 24 & 25
\end{vmatrix}$

Gunakan ekspansi kofaktor pada baris pertama:

$= 13
\begin{vmatrix}
19 & 20 \\
24 & 25
\end{vmatrix} - 14
\begin{vmatrix}
18 & 20 \\
23 & 25
\end{vmatrix} + 15
\begin{vmatrix}
18 & 19 \\
23 & 24
\end{vmatrix}$

Hitung determinan matriks 2×2:

$\begin{vmatrix}
19 & 20 \\
24 & 25
\end{vmatrix}
= (19 \times 25) - (20 \times 24) = 475 - 480 = -5$

$\begin{vmatrix}
18 & 20 \\
23 & 25
\end{vmatrix}
= (18 \times 25) - (20 \times 23) = 450 - 460 = -10$

$\begin{vmatrix}
18 & 19 \\
23 & 24
\end{vmatrix}
= (18 \times 24) - (19 \times 23) = 432 - 437 = -5$

Substitusi:

$= 13(-5) - 14(-10) + 15(-5)$

$= -65 + 140 - 75 = 0$

Karena semua submatriks 3×3 lainnya memiliki pola angka yang sama, maka determinan semua submatriks 3×3 adalah 0.

Karena setiap submatriks 4×4 memiliki determinan 0, maka:
$\det(C) = 1(0) - 2(0) + 3(0) - 4(0) + 5(0) = 0$

Jadi, determinan matriks 5×5 ini adalah 0
