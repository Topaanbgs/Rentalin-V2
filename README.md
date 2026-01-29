# 🏎️ Rentalin V2 - Premium PlayStation Rental Platform

**Rentalin V2** adalah evolusi dari sistem manajemen rental PlayStation yang kini hadir dengan arsitektur modern **Decoupled (Headless)**. Memisahkan antara performa tinggi **Next.js** di sisi frontend dan skalabilitas **Laravel API** di sisi backend untuk memberikan pengalaman pengguna yang premium dan responsif.

---

## 🚀 Live Production
🌍 [https://rentalin.site/](https://rentalin.site/)

---

## 🌟 What's New in V2?
- **Decoupled Architecture:** Frontend (Next.js) dan Backend (Laravel API) berjalan secara independen untuk performa dan keamanan optimal.
- **Automated Cronjobs:** Sistem otomasi untuk pengecekan status durasi rental dan keterlambatan pembayaran secara real-time menggunakan Laravel Task Scheduling.
- **Email Notifications:** Integrasi SMTP Mail Server untuk pengiriman informasi pendaftaran akun dan struk pembayaran otomatis kepada pengguna.
- **Modern State Management:** Implementasi Next.js caching dan hooks untuk memastikan navigasi halaman yang instan tanpa reload.

---

## 🛠️ Tech Stack

### Frontend
- **Framework:** Next.js 14+ (App Router)
- **Styling:** Tailwind CSS
- **Data Fetching:** Axios / SWR

### Backend (Core Engine)
- **Framework:** Laravel 10+ (Rest API)
- **Database:** MySQL
- **Automation:** Laravel Task Scheduling (Cronjobs)
- **Notification:** Laravel Mail / SMTP Integration

---

## ⚙️ Installation & Setup

Ikuti langkah-langkah di bawah ini untuk menjalankan project di lingkungan lokal:

### 1. Persiapan Backend (Laravel)

# Masuk ke folder backend
cd rentalin-backend

# Install dependencies
composer install

# Konfigurasi environment
cp .env.example .env
php artisan key:generate

# Jalankan database migration & seeder
php artisan migrate --seed

# Jalankan server backend
php artisan serve 

### 2. Persiapan Frontend (Next.js)

# Masuk ke folder frontend
cd rentalin-frontend

# Install dependencies
npm install

# Konfigurasi environment
cp .env.example .env

# Jalankan server frontend (development)
npm run dev

---

🔄 System Workflow (Cronjob & Notification)
Sistem ini menggunakan Laravel Task Scheduler yang berjalan setiap menit untuk melakukan audit otomatis terhadap transaksi:

Audit: Mengecek transaksi yang melewati batas waktu pembayaran.

Action: Mengubah status unit secara otomatis.

Notify: Mengirimkan notifikasi email otomatis kepada user terkait status akun atau tagihan mereka.

---

🎓 Academic Achievement
Proyek ini dikembangkan sebagai proyek akhir Mata Kuliah Teknologi Web dan berhasil meraih nilai "A". Fokus utama proyek ini adalah demonstrasi implementasi dynamic SEO, sistem terdistribusi, arsitektur API, dan otomasi layanan web.

Developed by Topan Bagus Prasetyo
