# Belajar HTML — html-basic

Repositori ini berisi contoh dan materi dasar HTML untuk pemula. Tujuannya adalah memberikan fondasi yang kuat tentang struktur dokumen HTML, tag dasar, praktik terbaik, dan contoh sederhana yang bisa langsung dijalankan di browser.

## Untuk siapa ini?
- Pemula yang baru mulai belajar web development.
- Programmer yang ingin menyegarkan kembali pengetahuan HTML.
- Siapa saja yang ingin memahami struktur halaman web sebelum belajar CSS dan JavaScript.

## Prasyarat
- Text editor (VS Code, Sublime, Notepad++, atau editor lain)
- Browser modern (Chrome, Firefox, Edge, Safari)
- Opsional: ekstensi Live Server untuk reload otomatis saat mengedit

## Struktur proyek (contoh)
- index.html — halaman contoh utama
- examples/ — contoh-contoh potongan kode HTML (forms, tables, lists)
- images/ — aset gambar yang digunakan pada contoh
- README.md — dokumentasi ini

(Ubah daftar di atas sesuai isi repositori Anda.)

## Cara menjalankan
1. Buka file `index.html` di browser: klik dua kali atau seret ke jendela browser.
2. Atau gunakan server lokal (rekomendasi untuk bekerja dengan fetch/asset path):
   - Dengan Python 3:
     ```bash
     python -m http.server 8000
     ```
     lalu buka http://localhost:8000
   - Dengan VS Code: gunakan ekstensi Live Server lalu klik "Go Live".

## Ringkasan materi HTML dasar

### Struktur dokumen HTML
```html
<!doctype html>
<html lang="id">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Judul Halaman</title>
  </head>
  <body>
    <!-- Konten halaman -->
  </body>
</html>
```

### Tag umum
- Headings: `<h1>` sampai `<h6>`
- Paragraf: `<p>`
- Link: `<a href="https://example.com">Tautan</a>`
- Gambar: `<img src="gambar.jpg" alt="Deskripsi">`
- List: `<ul>`, `<ol>`, `<li>`
- Table: `<table>`, `<tr>`, `<th>`, `<td>`
- Form: `<form>`, `<input>`, `<label>`, `<button>`
- Semantic: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`

### Atribut penting
- `id`, `class` — untuk styling dan scripting
- `alt` pada `<img>` — aksesibilitas
- `target="_blank"` pada `<a>` — membuka tab baru (gunakan `rel="noopener noreferrer"` untuk keamanan)

### Praktik aksesibilitas (singkat)
- Selalu isi `alt` pada gambar.
- Gunakan tag semantic untuk struktur.
- Pastikan kontras teks cukup tinggi.
- Gunakan label pada input form.

### Validasi dan best practices
- Validasi HTML di https://validator.w3.org
- Gunakan UTF-8 (`<meta charset="utf-8">`)
- Hindari penggunaan tag yang sudah deprecated
- Struktur konten secara logis untuk SEO dan aksesibilitas

## Contoh halaman sederhana
```html
<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Contoh Halaman</title>
</head>
<body>
  <header>
    <h1>Selamat datang</h1>
    <nav>
      <a href="#about">Tentang</a> |
      <a href="#contact">Kontak</a>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>Tentang HTML</h2>
      <p>HTML (HyperText Markup Language) adalah bahasa markup untuk membuat halaman web.</p>
    </section>

    <section id="contact">
      <h2>Kontak</h2>
      <form>
        <label for="name">Nama:</label>
        <input id="name" name="name" type="text" />
        <button type="submit">Kirim</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2026</p>
  </footer>
</body>
</html>
```

## Langkah belajar selanjutnya
1. Pelajari CSS untuk styling.
2. Pelajari JavaScript untuk interaksi.
3. Buat proyek kecil: halaman portofolio, halaman blog sederhana, atau form kontak.
4. Pelajari responsive design (media queries, flexbox, grid).

## Sumber belajar rekomendasi
- MDN Web Docs — HTML: https://developer.mozilla.org/en-US/docs/Web/HTML
- W3C Validator: https://validator.w3.org
- HTML Living Standard: https://html.spec.whatwg.org

## Lisensi
Lisensi proyek ini bebas digunakan. Sesuaikan jika mau menambahkan lisensi tertentu (MIT, Apache, dsb).

## Penulis
ARIEL-SIMANJUNTAK — repositori: ARIEL-SIMANJUNTAK/html-basic

Terima kasih sudah menggunakan repo ini! Semoga membantu perjalanan belajarmu dalam membangun halaman web dengan HTML.
