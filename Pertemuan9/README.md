# Dashboard Akademik

Tugas Praktikum Desain Web — Pertemuan 9

Halaman dashboard sederhana untuk memantau data mahasiswa Program Studi Teknik Informatika pada Semester Gasal 2026/2027. Halaman dibuat dengan HTML dan **Bootstrap 5** serta sedikit CSS buatan sendiri, dan tampilannya responsif di HP, tablet, maupun laptop.

## Identitas

| | |
|---|---|
| Nama | Ardhelia |
| NPM | 4525210092 |
| Mata Kuliah | Desain Web (Praktikum) |
| Semester | Gasal 2026/2027 |

## Struktur Folder

```
Tugas/
├── index.html   # Halaman utama (struktur & isi dashboard)
├── style.css    # CSS buatan sendiri (dimuat setelah Bootstrap)
└── README.md    # Dokumentasi proyek
```

## Fitur dan Komponen

### 1. Header
Judul "Dashboard Akademik" dengan subjudul program studi dan semester, menggunakan latar `bg-primary` dan teks putih.

### 2. Empat Kartu Statistik
Menampilkan ringkasan data dalam bentuk kartu (`card`):

| Kartu | Nilai | Warna |
|---|---|---|
| Total Mahasiswa | 240 | Biru (`text-primary`) |
| Mata Kuliah | 36 | Hijau (`text-success`) |
| Rata-rata IPK | 3,42 | Kuning (`text-warning`) |
| Dosen Pengajar | 18 | Merah (`text-danger`) |

Tata letak kartu memakai grid Bootstrap sehingga jumlah kolomnya menyesuaikan lebar layar:

| Perangkat | Kelas | Jumlah Kolom |
|---|---|---|
| HP | `col-12` | 1 kolom |
| Tablet | `col-md-6` | 2 kolom |
| Laptop | `col-lg-3` | 4 kolom |

### 3. Tabel Data Mahasiswa
Tabel berisi 10 data mahasiswa dengan kolom **No, NIM, Nama, Program Studi, Semester, IPK, Status, dan Aksi**.

- `table-striped` dan `table-hover` untuk baris belang dan efek sorot saat kursor lewat.
- `table-responsive` agar tabel bisa digeser ke samping pada layar kecil.
- Kolom **Status** memakai *badge* berwarna:
  - 🟢 **Aktif** (`bg-success`)
  - 🟡 **Cuti** (`bg-warning`)
  - 🔵 **Lulus** (`bg-info`)
  - 🔴 **Nonaktif** (`bg-danger`)
- Tombol **+ Tambah Mahasiswa** dan **Detail** pada tiap baris (saat ini hanya tampilan, belum memiliki fungsi).

### 4. Footer
Keterangan hak cipta dan identitas tugas dengan latar `bg-dark`.

## CSS Buatan Sendiri (`style.css`)

| Selector | Fungsi |
|---|---|
| `.angka` | Mengatur angka pada kartu statistik (ukuran `2.5rem`, tebal, tanpa margin bawah) |
| `.card` | Menghilangkan garis tepi bawaan kartu Bootstrap |
| `.card:hover` | Kartu naik sedikit (`translateY(-3px)`) dengan transisi 0,2 detik saat disorot kursor |

## Teknologi

- HTML5
- CSS3
- [Bootstrap 5.3.3](https://getbootstrap.com/) (dimuat lewat CDN jsDelivr)
  - CSS dipanggil di `<head>`
  - JavaScript (bundle) dipanggil di bagian bawah `<body>`

## Cara Menjalankan

1. Ekstrak `Tugas.zip` sehingga folder `Tugas/` muncul.
2. Buka file `index.html` dengan browser (Chrome, Firefox, Edge, dll.).
3. Pastikan perangkat **terhubung ke internet**, karena Bootstrap dimuat lewat CDN.

Untuk mencoba tampilan responsif, ubah ukuran jendela browser atau gunakan mode *Device Toolbar* di DevTools (tekan `F12`, lalu `Ctrl + Shift + M`).

## Catatan

- Data pada dashboard bersifat statis (ditulis langsung di HTML) sebagai contoh.
- Tombol **Tambah Mahasiswa** dan **Detail** belum terhubung ke fitur apa pun.
