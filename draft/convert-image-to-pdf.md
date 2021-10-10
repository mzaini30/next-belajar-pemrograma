# Convert Image to PDF

Install dulu ImageMagick:

```bash
sudo apt install imagemagick
```

Lalu, atur supaya bisa convert ke PDF:

```bash
sudo subl /etc/ImageMagick-6/policy.xml
```

Perhatikan pada bagian:

```xml
<policy domain="coder" rights="none" pattern="PDF" />
```

Ubah menjadi:

```xml
<policy domain="coder" rights="read|write" pattern="PDF" />
```

Lalu, untuk convertnya, misal `a.jpg` menjadi `a.pdf`:

```bash
convert a.jpg a.pdf
```