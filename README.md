# PCD_Assignment03

Tugas ini mengimplementasikan metode segmentasi **region growing** dan operasi **morfologi** (erosi, dilasi, opening, closing), lalu membandingkan hasil segmentasi sebelum dan sesudah morfologi diterapkan.

## Notebook

Link Google Colab: [Here](https://colab.research.google.com/drive/1LGddozSi-agYRid2q07LzzJ4Th98IdK_?usp=sharing)

## Isi

- **Region growing** dengan kriteria `|I(p) - I(q)| < T`, seed dipilih acak sampai seluruh piksel memiliki region.
- **Studi ablasi** nilai T = 4, 6, 8, 10, 12.
- **Operasi morfologi** dengan structuring element 3×3: erosi, dilasi, opening, dan closing.
- **Citra uji**: `coins`, `page`, `camera`, dan potongan `hubble_deep_field` dari scikit-image.

## Library

NumPy dipakai untuk operasi array, Pillow untuk membaca dan menyimpan gambar, Matplotlib untuk visualisasi, dan scikit-image **hanya** untuk mengambil gambar contoh. Seluruh algoritme segmentasi dan morfologi ditulis sendiri.
