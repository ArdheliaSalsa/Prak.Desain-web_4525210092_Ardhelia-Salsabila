# Arunika Studio

Landing page sederhana untuk Arunika Studio yang dibuat menggunakan HTML dan CSS.

## Struktur Folder

```text
arunika_studio/
├── index.html
├── style.css
└── README.md
```

## Fitur

- Header dengan navigasi Home, Layanan, dan Kontak.
- Hero section dengan judul, deskripsi, dan tombol.
- Tiga card layanan: Desain Kreatif, Fotografi, dan Solusi Digital.
- Bagian kontak dan footer.
- CSS dipisahkan dari HTML.
- Menggunakan box model melalui `box-sizing: border-box`.
- Menggunakan class reusable seperti `.container`, `.button`, dan `.section`.
- Responsive design dengan media query pada layar di bawah 768px.
- Tiga card layanan berubah menjadi satu kolom pada layar kecil.

## Cara Menjalankan

1. Unduh atau salin folder project.
2. Pastikan `index.html` dan `style.css` berada di folder yang sama.
3. Buka file `index.html` menggunakan browser.
4. Untuk memeriksa tampilan mobile, buka Developer Tools pada browser dan aktifkan device toolbar.

## Penjelasan Responsive Design

Pada layar desktop, `.service-grid` menggunakan tiga kolom dengan CSS Grid. Ketika lebar layar kurang dari 768px, media query mengubahnya menjadi `grid-template-columns: 1fr`, sehingga setiap card tampil dalam satu kolom.

## Catatan

Alamat email pada tombol kontak (`hello@arunikastudio.com`) merupakan contoh dan dapat diganti sesuai kebutuhan.
