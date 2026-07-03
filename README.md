LKPD Generator AI

Aplikasi SaaS (Software as a Service) berbasis web untuk menghasilkan Lembar Kerja Peserta Didik (LKPD) profesional menggunakan kecerdasan buatan (Google Gemini AI).

Aplikasi ini dibangun menggunakan HTML5 murni, CSS3, dan Vanilla JavaScript di bagian Frontend, serta Node.js (Vercel Serverless Functions) di bagian Backend untuk menyembunyikan API Key dengan aman.

🚀 Fitur Utama

Single Page Application (SPA) murni tanpa framework, navigasi super cepat.

Generator Pintar: Konfigurasi jenjang, mapel, P5, jumlah soal, dan jenis soal.

Live Preview: Pratinjau hasil berformat kertas A4 (Markdown di-render ke HTML).

Export to Word: Unduh hasil LKPD langsung menjadi file .docx siap cetak.

Riwayat Lokal: Menyimpan riwayat LKPD otomatis di LocalStorage peramban.

Keamanan Keamanan: Kode Akses AIGENLKPD21 untuk login, dan backend serverless untuk melindungi API key.

📂 Struktur Proyek

LKPD-Generator-AI/
│
├── index.html         # (UI Utama: Menggabungkan HTML, CSS, JS)
├── README.md          # Dokumentasi ini
├── vercel.json        # Konfigurasi Vercel (Routes & Builders)
├── .gitignore         # File yang diabaikan Git
├── .env.example       # Contoh variabel lingkungan
│
└── api/
    └── generate.js    # Vercel Serverless Function penghubung Gemini API


🛠️ Instalasi & Penggunaan Lokal (Tanpa Vercel)

Karena menggunakan Vercel Serverless Functions (/api/generate), untuk menjalankannya secara lokal Anda membutuhkan Vercel CLI:

Clone repositori ini.

Install Vercel CLI: npm i -g vercel

Salin file environment: cp .env.example .env

Isi GEMINI_API_KEY di file .env dengan API key Anda dari Google AI Studio.

Jalankan lokal server: vercel dev

Buka URL yang diberikan (biasanya localhost:3000).

(Gunakan kode akses: AIGENLKPD21 untuk masuk).

🚀 Panduan Deploy ke GitHub

Buat repositori baru di GitHub (kosong, tanpa README/License).

Buka terminal di folder proyek ini dan inisialisasi Git:

git init
git add .
git commit -m "Initial commit: LKPD Generator AI"
git branch -M main
git remote add origin https://github.com/USERNAME_ANDA/NAMA_REPO_ANDA.git
git push -u origin main


☁️ Panduan Deploy ke Vercel

Buat akun atau login ke Vercel.com.

Klik tombol Add New... -> Project.

Hubungkan akun GitHub Anda dan Import repositori yang baru saja Anda push.

Pada bagian Environment Variables, tambahkan:

Name: GEMINI_API_KEY

Value: [Masukkan API Key Google Gemini Anda]

Klik Deploy.

Selesai! Aplikasi LKPD Generator AI Anda sudah online dan aman digunakan.