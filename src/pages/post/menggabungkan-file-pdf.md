---
kategori: Linux
judul: Menggabungkan File PDF
---

Install dulu `pdftk`:

```bash
sudo apt install pdftk
```

Misal, kita ingin menggabungkan `a.pdf` dengan `b.pdf` menjadi `c.pdf`, maka perintahnya adalah:

```bash
pdftk a.pdf b.pdf cat output c.pdf
```