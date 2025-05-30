Learn-Web-Development-Intermediate
Dicerita — Aplikasi Berbagi Cerita
StoryGan adalah aplikasi web Single-Page Application (SPA) yang memungkinkan pengguna untuk membaca dan membagikan cerita mereka dari berbagai lokasi. Aplikasi ini dibangun dengan memanfaatkan Web API dan teknologi front-end modern.

🎯 Fitur Utama
✅ Mengambil data cerita dari Story API
✅ Menampilkan daftar cerita dengan gambar dan deskripsi
✅ Peta interaktif untuk menunjukkan lokasi cerita dengan marker dan popup
✅ Formulir untuk menambahkan cerita baru (dengan akses kamera & map click)
✅ Aksesibilitas sesuai WCAG: skip to content, label pada input, teks alternatif, semantic HTML
✅ Transisi halaman halus dengan View Transition API

🛠️ Teknologi dan Tools
HTML5, CSS3, JavaScript
Web API (Story API)
Leaflet.js untuk peta digital
View Transition API
Model-View-Presenter (MVP) Pattern
Font Awesome untuk ikon
Web Camera API untuk ambil gambar
MediaDevices & Geolocation API
🌐 SPA Routing
Routing dilakukan menggunakan hash (#) untuk memuat:

Halaman utama (#/)
Tambah cerita (#/add)
Detail cerita (#/story/:id)
🗺️ Integrasi Peta
Menggunakan Leaflet.js
Menampilkan marker di lokasi cerita
Popup berisi ringkasan cerita
Saat tambah cerita, pengguna dapat klik di peta untuk mengambil latitude dan longitude
Mendukung layer control dan beberapa gaya tile map
📷 Akses Kamera
Fitur ambil gambar saat menambahkan cerita
Menggunakan MediaDevices.getUserMedia()
Stream otomatis dimatikan setelah pengambilan gambar selesai
✅ Aksesibilitas
Skip to content di awal halaman
Setiap gambar memiliki alt text
Setiap <input> memiliki label terkait
Gunakan elemen semantic seperti <main>, <nav>, <section>, <header>
🌈 Tampilan Menarik
Palet warna diambil dari colorhunt.co
Tata letak responsif dan mobile-friendly
Font yang mudah dibaca
Margin dan padding proporsional
Ikon-ikon visual untuk meningkatkan UX
🚀 Cara Menjalankan Proyek
Clone repositori ini:
git clone https://github.com/aldiyanson/Belajar-Pengembangan-Web-Intermediate-Proyek-Kedua


# App Starter Project with Webpack

Proyek ini adalah setup dasar untuk aplikasi web yang menggunakan webpack untuk proses bundling, Babel untuk transpile JavaScript, serta mendukung proses build dan serving aplikasi.

## Table of Contents

- [Getting Started](#getting-started)
- [Scripts](#scripts)
- [Project Structure](#project-structure)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (disarankan versi 12 atau lebih tinggi)
- [npm](https://www.npmjs.com/) (Node package manager)

### Installation

1. Download starter project [di sini](https://raw.githubusercontent.com/dicodingacademy/a219-web-intermediate-labs/099-shared-files/starter-project-with-webpack.zip).
2. Lakukan unzip file.
3. Pasang seluruh dependencies dengan perintah berikut.
   ```shell
   npm install
   ```

## Scripts

- Build for Production:
  ```shell
  npm run build
  ```
  Script ini menjalankan webpack dalam mode production menggunakan konfigurasi `webpack.prod.js` dan menghasilkan sejumlah file build ke direktori `dist`.

- Start Development Server:
  ```shell
  npm run start-dev
  ```
  Script ini menjalankan server pengembangan webpack dengan fitur live reload dan mode development sesuai konfigurasi di`webpack.dev.js`.

- Serve:
  ```shell
  npm run serve
  ```
  Script ini menggunakan [`http-server`](https://www.npmjs.com/package/http-server) untuk menyajikan konten dari direktori `dist`.

## Project Structure

Proyek starter ini dirancang agar kode tetap modular dan terorganisir.

```text
starter-project/
├── dist/                   # Compiled files for production
├── src/                    # Source project files
│   ├── public/             # Public files
│   ├── scripts/            # Source JavaScript files
│   │   └── index.js        # Main JavaScript entry file
│   ├── styles/             # Source CSS files
│   │   └── styles.css      # Main CSS file
│   └── index.html/         # Main HTML file
├── package.json            # Project metadata and dependencies
├── package-lock.json       # Project metadata and dependencies
├── README.md               # Project documentation
├── STUDENT.txt             # Student information
├── webpack.common.js       # Webpack common configuration
├── webpack.dev.js          # Webpack development configuration
└── webpack.prod.js         # Webpack production configuration
```
