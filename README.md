# Segmentasi Pelanggan Mall dengan K-Means

Repositori ini berisi proyek segmentasi pelanggan menggunakan algoritma **K-Means Clustering** pada dataset **Mall Customer Segmentation**. Tujuan dari proyek ini adalah untuk mengelompokkan pelanggan berdasarkan pendapatan tahunan dan skor pengeluaran mereka, sehingga membantu bisnis dalam memahami karakteristik pelanggan dan merancang strategi pemasaran yang lebih efektif.

## 1. Struktur Dataset
Dataset ini terdiri dari 200 baris dan 5 kolom, yaitu:
- **CustomerID:** ID unik untuk setiap pelanggan (tipe data `int64`)
- **Gender:** Jenis kelamin pelanggan (tipe data `object`)
- **Age:** Usia pelanggan dalam tahun (tipe data `int64`)
- **Annual Income (k$):** Pendapatan tahunan pelanggan dalam ribuan dolar (tipe data `int64`)
- **Spending Score (1-100):** Skor pengeluaran pelanggan berdasarkan perilaku belanja (tipe data `int64`)

## 2. Penentuan Jumlah Cluster (Metode Elbow)
Untuk menentukan jumlah cluster yang optimal, digunakan **metode Elbow** dari jumlah 1-10.  
Hasil analisis menunjukkan bahwa:
- **Jumlah cluster optimal:** 4
- **Total WCSS (Within-Cluster Sum of Squares):** 73.679,789

Empat cluster dipilih karena memberikan keseimbangan terbaik antara meminimalkan variasi dalam cluster dan memaksimalkan perbedaan antar cluster.

## 3. Nilai Centroid untuk Setiap Cluster
Berikut adalah nilai centroid hasil training K-Means untuk setiap cluster:
![image](https://github.com/user-attachments/assets/360f521f-3f33-4197-be04-a8fbc7f3d5ae)

- **Cluster 1:**  
  - Pendapatan tahunan: **$48.260**
  - Skor pengeluaran: **56,48**  
  - **Karakteristik:** Pendapatan menengah, belanja tinggi.

- **Cluster 2:**  
  - Pendapatan tahunan: **$86.540**
  - Skor pengeluaran: **82,13**  
  - **Karakteristik:** Pendapatan tinggi, belanja intensif.

- **Cluster 3:**  
  - Pendapatan tahunan: **$87.000**
  - Skor pengeluaran: **18,63**  
  - **Karakteristik:** Pendapatan tinggi, belanja rendah.

- **Cluster 4:**  
  - Pendapatan tahunan: **$26.300**
  - Skor pengeluaran: **20,91**  
  - **Karakteristik:** Pendapatan rendah, belanja rendah.

## 💡 Kredit
Dwi Cahya Novita. Proyek ini adalah bagian dari kursus **Machine Learning untuk Pemula** yang diselenggarakan oleh **Dicoding**.

---
