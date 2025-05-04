---
title: Transformasi Linear

---

# Transformasi linier

Transformasi linier adalah konsep fundamental dalam aljabar linear yang menggambarkan pemetaan antara dua ruang vektor dengan mempertahankan struktur liniernya. Artinya, transformasi ini memetakan vektor dari satu ruang ke ruang lain sedemikian rupa sehingga operasi penjumlahan vektor dan perkalian skalar tetap berlaku.

Secara formal, misalkan terdapat dua ruang vektor, $V$ dan $W$, serta sebuah fungsi $T: V \rightarrow W$. Fungsi $T$ disebut transformasi linier jika memenuhi dua sifat berikut:

1. **Additivitas**: $T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$ untuk semua $\mathbf{u}, \mathbf{v} \in V$.
2. **Homogenitas**: $T(k\mathbf{u}) = kT(\mathbf{u})$ untuk semua skalar $k$ dan $\mathbf{u} \in V$.

Jika kedua sifat ini terpenuhi, maka $T$ adalah transformasi linier.&#x20;

Contoh transformasi linier meliputi rotasi, dilatasi, refleksi, proyeksi, dan perkalian matriks. Misalnya, fungsi $T: \mathbb{R}^2 \rightarrow \mathbb{R}^2$ yang didefinisikan oleh $T(x, y) = (2x, 3y)$ adalah transformasi linier karena memenuhi kedua sifat di atas.

Transformasi linier dapat direpresentasikan menggunakan matriks. Jika $T$ adalah transformasi linier dari $\mathbb{R}^n$ ke $\mathbb{R}^m$, maka terdapat matriks $A$ berukuran $m \times n$ sehingga untuk setiap vektor $\mathbf{x} \in \mathbb{R}^n$, berlaku $T(\mathbf{x}) = A\mathbf{x}$.

Transformasi linier memiliki berbagai aplikasi dalam berbagai bidang, seperti grafika komputer untuk melakukan transformasi gambar, fisika dalam analisis sistem linear, ekonomi dalam pemodelan input-output, dan statistika dalam analisis regresi.

## Pembuktian Transformasi Rotasi Bidang

![WhatsApp Image 2025-04-28 at 09.11.12_a8f8ac4f](https://hackmd.io/_uploads/B1s9qWBllg.jpg)


Kita ingin membuktikan bahwa transformasi linier $T: \mathbb{R}^2 \to \mathbb{R}^2$ yang merepresentasikan rotasi berlawanan arah jarum jam sebesar sudut $\theta$, bisa dinyatakan dengan matriks:

$$
A = 
\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
$$

## Langkah-langkah Pembuktian

1. Misalkan kita punya vektor $\mathbf{v} = (x, y)$. Kita bisa ubah ke bentuk koordinat polar:

$$
\mathbf{v} = (x, y) = (r \cos \alpha, r \sin \alpha)
$$

Di mana:
- $r$ adalah panjang dari vektor $\mathbf{v}$
- $\alpha$ adalah sudut antara vektor $\mathbf{v}$ dan sumbu-x positif

2. Jika vektor tersebut diputar sebesar $\theta$, maka posisinya menjadi:

$$
\mathbf{v'} = (r \cos(\alpha + \theta),\ r \sin(\alpha + \theta))
$$

3. Gunakan identitas trigonometri sudut jumlah:

$$
\cos(\alpha + \theta) = \cos \alpha \cos \theta - \sin \alpha \sin \theta
$$
$$
\sin(\alpha + \theta) = \sin \alpha \cos \theta + \cos \alpha \sin \theta
$$

Maka:

$$
\mathbf{v'} = r 
\begin{bmatrix}
\cos \alpha \cos \theta - \sin \alpha \sin \theta \\
\sin \alpha \cos \theta + \cos \alpha \sin \theta
\end{bmatrix}
$$

4. Karena $x = r \cos \alpha$ dan $y = r \sin \alpha$, maka:

$$
\mathbf{v'} = 
\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

Artinya, rotasi memang dapat direpresentasikan oleh matriks di atas.
