# Praktik Machine Learning – OpenCV Image Processing

## Deskripsi
Repository ini berisi hasil praktik **Machine Learning menggunakan OpenCV pada Python** yang mempelajari dasar-dasar **pengolahan citra digital (Image Processing)**.

Praktikum ini dilakukan berdasarkan video pembelajaran:

**OpenCV – Crop, Resize & Blending Image**

Pada praktikum ini dilakukan beberapa teknik pengolahan gambar seperti:

- Crop Image
- Resize Image
- Image Blending
- Overlay Object

menggunakan library **OpenCV**.

Tujuan dari praktikum ini adalah untuk memahami dasar **Computer Vision** yang sering digunakan dalam berbagai aplikasi seperti **face recognition, object detection, dan image processing**.

---

## Teknologi yang Digunakan

- Python
- OpenCV (`cv2`)
- NumPy
- Jupyter Notebook
- VsCode

---

## Struktur Repository

```bash
Tugas_Kelompok_2_ML/
│
├── OpenCV_2.ipynb
├──  /
│   ├── sunflower.jpg
│   ├── burung_macaw.jpg
│   ├── olat_maras.jpeg
│   └── Gunung_Bromo.jpg
│
├── results/
│   ├── Overlay Image.png
│   ├── Resized Image.png
│   ├── Blending Result.png
│   └── Resized Image_screenshot.png
│
└── README.md
```

---

## Langkah Praktikum

### 1. Import Library

Library yang digunakan pada praktikum ini adalah **OpenCV dan NumPy**.

```python
import cv2
import numpy as np
```

OpenCV digunakan untuk **pengolahan citra**, sedangkan NumPy digunakan untuk **manipulasi data gambar dalam bentuk array**.

---

### 2. Image Crop

Crop digunakan untuk mengambil bagian tertentu dari gambar.

Contoh kode:

```python
img_crop = img[y1:y2, x1:x2]
```

Metode ini menggunakan **NumPy slicing** untuk menentukan area gambar yang akan diambil.

---

### 3. Image Resize

Resize digunakan untuk mengubah ukuran gambar.

Contoh kode:

```python
img_resize = cv2.resize(img, (w, h))
```

Resize dapat dilakukan untuk **memperkecil atau memperbesar ukuran gambar** sesuai kebutuhan.

---

### 4. Image Blending

Blending digunakan untuk menggabungkan dua gambar dengan tingkat transparansi tertentu.

Contoh kode:

```python
blending_img = cv2.addWeighted(img1, alpha, img2, beta, 0)
```

Keterangan:

- **alpha** → transparansi gambar pertama  
- **beta** → transparansi gambar kedua  

---

### 5. Overlay Object

Overlay digunakan untuk menambahkan objek transparan pada gambar.

Contoh kode:

```python
overlay = np.zeros_like(img)
overlay[10:300, 10:50, 1] = 255
```

Kode tersebut membuat **objek overlay berwarna pada area tertentu pada gambar**.

---


## Video Presentasi

Link Video Presentasi YouTube:
# https://youtu.be/q5YJyNpMsnw
---

## Kesimpulan

Dari praktikum ini dapat disimpulkan bahwa **OpenCV** merupakan library yang sangat powerful untuk **pengolahan citra digital menggunakan Python**.

Beberapa teknik dasar yang dipelajari dalam praktikum ini adalah:

- Crop Image
- Resize Image
- Image Blending
- Overlay Object

Teknik-teknik tersebut merupakan dasar penting dalam pengembangan **Computer Vision dan Machine Learning berbasis citra**.

## Anggota Kelompok

1. Alfadrian Januarsyah (231001067)
2. Tasri Zulfitriyati (231001074)
3. M. Irvan Maualana Putra (231001071)
4. Nabila Isnaeni (231001054)
5. Silvia Fasya Aprilian (231001002)
