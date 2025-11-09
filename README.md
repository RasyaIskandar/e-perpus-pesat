# E-Perpus Pesat

E-Perpus Pesat adalah aplikasi manajemen perpustakaan berbasis web yang digunakan untuk mengelola data buku, peminjaman, pengembalian, serta akun pengguna. Sistem ini dibuat menggunakan Laravel dan Tailwind CSS dengan autentikasi login untuk admin dan anggota perpustakaan.

---

## ✨ Fitur Utama

| Fitur | Deskripsi |
|------|-----------|
| Login & Register | Sistem autentikasi untuk pengguna dan admin |
| CRUD Buku | Tambah, edit, hapus, dan lihat detail buku |
| Peminjaman Buku | Anggota dapat meminjam buku sesuai stok tersedia |
| Pengembalian Buku | Admin/anggota dapat mengembalikan buku |
| Perpanjang Peminjaman | Perpanjangan tanggal kembali buku |
| Pengembalian Paksa | Admin dapat memaksa status buku kembali jika diperlukan |
| Riwayat Peminjaman | Data peminjaman lengkap untuk admin |

---

## 🏗️ Teknologi yang Digunakan

| Teknologi | Keterangan |
|----------|-----------|
| Laravel 10+ | Backend & Routing |
| Tailwind CSS | UI/Styling |
| MySQL | Database |
| Blade Templates | Frontend View |
| Auth Laravel Breeze | Sistem Login/Register |

---

## 📦 Instalasi & Setup

Pastikan sudah terinstall:
- PHP 8.1+
- Composer
- MySQL / MariaDB
- Node.js

### 1. Clone Repository
git clone https://github.com/RasyaIskandar/e-perpus-pesat.git
cd e-perpus-pesat

shell
Salin kode

### 2. Install Dependencies
composer install
npm install
npm run dev

shell
Salin kode

### 3. Copy Konfigurasi `.env`
cp .env.example .env

shell
Salin kode

### 4. Generate Key & Konfigurasi Database
php artisan key:generate

bash
Salin kode
Edit `.env` → sesuaikan database.

### 5. Migrasi & Seeder (jika ada)
php artisan migrate --seed

shell
Salin kode

### 6. Jalankan Server
php artisan serve

yaml
Salin kode

---

## 👤 Role Pengguna

| Role | Hak Akses |
|------|-----------|
| Admin | Kelola buku, kelola pengembalian, lihat riwayat |
| Anggota | Pinjam buku, perpanjang, kembalikan |

---

## 📚 Struktur Direktori Penting

app/Http/Controllers/anggotaController.php
app/Http/Controllers/bookController.php
resources/views/
routes/web.php

yaml
Salin kode

---

## 🚀 Rencana Pengembangan

- Notifikasi WA ketika pinjam/kembali buku
- QR Code scan buku
- Dashboard statistik pinjaman

---

## 👨‍💻 Developer
**Rasya Iskandar**  
SMK Informatika Pesat — RPL  
⚡ Cara Push ke GitHub (Singkat)
Jalankan di folder project

csharp
Salin kode
git init
git add .
git commit -m "First commit - E-Perpus Pesat"
git branch -M main
git remote add origin https://github.com/RasyaIskandar/e-perpus-pesat.git
git push -f origin main
Kenapa pakai -f?
Karena repo GitHub tadi sudah berisi file default, jadi perlu force overwrite.

