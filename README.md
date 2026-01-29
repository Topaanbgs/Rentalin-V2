# 🏎️ Rentalin V2 - Premium PlayStation Rental Platform

**Rentalin V2** adalah evolusi dari sistem manajemen rental PlayStation yang kini hadir dengan arsitektur modern **Decoupled (Headless)**. Memisahkan antara performa tinggi **Next.js** di sisi frontend dan skalabilitas **Laravel API** di sisi backend.

---

## 🚀 Live Production
🌍 [https://rentalin.site/](https://rentalin.site/)

---

## 🌟 What's New in V2?
- **Decoupled Architecture:** Frontend (Next.js) dan Backend (Laravel API) berjalan secara independen untuk performa optimal.
- **Automated Cronjobs:** Sistem otomatis untuk pengecekan status durasi rental dan keterlambatan pembayaran secara real-time.
- **Email Notifications:** Integrasi Mail Server untuk pengiriman informasi pendaftaran akun dan pengingat pembayaran otomatis kepada pengguna.
- **Advanced State Management:** Menggunakan Next.js caching dan hooks untuk pengalaman pengguna yang sangat responsif.

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

## 📸 System Architecture

---

## ⚙️ Installation & Setup

### 1. Backend (Laravel)
```bash
cd rentalin-backend
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve

### 2. Frontend (Next.js)
Bash
cd rentalin-frontend
npm install
cp .env.example .env
npm run dev

🎓 Academic Achievement
Proyek ini dikembangkan sebagai proyek akhir Mata Kuliah Teknologi Web dan berhasil meraih nilai "A". Fokus utama proyek adalah implementasi sistem terdistribusi dan otomasi layanan web.

Developed by Topan Bagus Prasetyo
