Laporan Proyek Website Inventory Barang
1. Judul Proyek
Sistem Informasi Inventaris Barang Berbasis Web Menggunakan PHP dan Tailwind CSS

2. Deskripsi Proyek
Website ini merupakan sistem informasi inventaris barang yang dirancang untuk membantu pengelolaan data barang dalam suatu organisasi atau instansi. Pengguna dapat melakukan input, update, hapus, dan pencarian data barang secara mudah dan efisien. Sistem ini dilengkapi dengan fitur filtering berdasarkan kategori, pencarian, pagination, serta export data ke file CSV dan PDF.

3. Fitur-Fitur Utama
Berikut adalah fitur-fitur utama dalam sistem:

Manajemen Barang

Tambah, edit, dan hapus data barang.

Menyimpan informasi nama barang, kategori, jumlah stok, harga, dan tanggal masuk.

Manajemen Kategori

Tambah, edit, dan hapus kategori barang.

Kategori dihubungkan dengan barang melalui relasi kategori_id.

Pencarian dan Filter

Fitur pencarian berdasarkan nama barang atau nama kategori.

Filter berdasarkan kategori barang.

Pagination

Menampilkan data per halaman dengan navigasi halaman otomatis.

Export Data

Export data barang ke file CSV dan PDF.

Desain Modern

Menggunakan Tailwind CSS dengan tampilan dark mode yang modern dan responsif.

Notifikasi Interaktif

Menggunakan SweetAlert2 untuk menampilkan notifikasi setelah update data.

4. Struktur Database
Database inventaris_barang terdiri dari dua tabel utama:

4.1. Tabel kategori

Field	Tipe Data	Keterangan
id	INT (PK, AI)	Primary key
nama_kategori	VARCHAR(100)	Nama kategori barang
4.2. Tabel barang

Field	Tipe Data	Keterangan
id	INT (PK, AI)	Primary key
nama_barang	VARCHAR(100)	Nama barang
kategori_id	INT (FK)	Relasi ke tabel kategori
jumlah_stok	INT	Jumlah stok barang
harga_barang	DECIMAL	Harga satuan barang
tanggal_masuk	DATE	Tanggal barang masuk
5. File-File Utama

Nama File	Fungsi
index.php	Halaman utama, menampilkan tabel barang, pencarian, filter, pagination
tambah.php	Form untuk menambah barang baru
edit.php	Form untuk mengedit data barang
hapus.php	Proses penghapusan barang
kategori.php	Manajemen kategori (tambah, edit, hapus)
edit_kategori.php	Form edit kategori
export.php	Export data ke CSV
export_pdf.php	Export data ke PDF menggunakan DomPDF
koneksi.php	File koneksi ke database
6. Teknologi yang Digunakan
Frontend: HTML5, Tailwind CSS

Backend: PHP

Database: MySQL

Library Tambahan:

SweetAlert2 (notifikasi)

DomPDF (export PDF)

Tabler Icons (ikon UI)

7. Cara Penggunaan
Login (jika ditambahkan autentikasi)

Navigasi ke halaman utama index.php.

Tambahkan kategori terlebih dahulu di kategori.php.

Tambahkan barang melalui tombol +Barang.

Gunakan fitur pencarian dan filter untuk menemukan barang.

Gunakan tombol Export untuk mendownload data barang.

8. Pengembangan Selanjutnya
Menambahkan fitur login dan autentikasi user.

Penambahan fitur role admin dan user.

Menambahkan dashboard statistik barang.

Validasi form lebih lanjut di sisi server maupun client.

