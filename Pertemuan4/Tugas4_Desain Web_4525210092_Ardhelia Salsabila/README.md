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

## Output
### Before
<img width="1128" height="1038" alt="Screenshot 2026-10-12 132102" src="https://github.com/user-attachments/assets/b8156b0f-8a90-42cd-a059-00657c77d552" />

### After
<img width="1911" height="1021" alt="Screenshot 2026-10-12 132347" src="https://github.com/user-attachments/assets/e66358a7-dbe9-46fd-ae5e-da74acdfec68" />
<img width="1916" height="1023" alt="Screenshot 2026-10-12 132400" src="https://github.com/user-attachments/assets/e3e58bb6-da19-4d64-8ca5-3829714e8b7c" />


## Penjelasan Responsive Design

Pada layar desktop, `.service-grid` menggunakan tiga kolom dengan CSS Grid. Ketika lebar layar kurang dari 768px, media query mengubahnya menjadi `grid-template-columns: 1fr`, sehingga setiap card tampil dalam satu kolom.

## Catatan

Alamat email pada tombol kontak (`hello@arunikastudio.com`) merupakan contoh dan dapat diganti sesuai kebutuhan.
