# WARUNG_HAYDAY

Sistem pemesanan produk Hay Day berbasis HTML, CSS, JavaScript, Google Sheets, dan Google Apps Script.

Project ini dirancang untuk memudahkan penjualan item Hay Day dengan fitur checkout otomatis, dashboard admin, manajemen harga produk, serta penyimpanan pesanan langsung ke Google Spreadsheet.

---

## Fitur
* Checkout produk BEM, SEM, dan LEM
* Harga produk dinamis melalui Google Sheets
* Integrasi Google Apps Script API
* Penyimpanan data pesanan ke Google Spreadsheet
* Dashboard Admin
* Filter pesanan berdasarkan produk
* Nofitikasi email
* Tombol salin tag akun
* Tombol selesai pesanan
* Integrasi WhatsApp
* Integrasi QRIS pembayaran
* Tampilan mobile friendly
* Siap digunakan di Cloudflare Pages

### Checkout Produk

* Checkout BEM, SEM, dan LEM
* Minimal pembelian 2 tag
* Perhitungan total otomatis
* Tombol salin nominal pembayaran
* Integrasi QRIS
* Integrasi WhatsApp

### Dashboard Admin

* Melihat seluruh pesanan
* Filter berdasarkan produk
* Tombol salin daftar tag
* Tombol tandai pesanan selesai
* Statistik pesanan pending
* Pengaturan produk

### Pengaturan Produk

* Ubah nama produk
* Ubah harga produk
* Harga otomatis tersinkron ke website
* Tidak perlu mengedit file HTML

### Database

* Google Spreadsheet sebagai database utama
* Data pesanan tersimpan otomatis
* Status pesanan (PENDING / SELESAI)

### Tampilan

* Mobile Friendly
* Siap digunakan di Cloudflare Pages
* Desain sederhana dan ringan

---

## Teknologi

* HTML5
* CSS3
* JavaScript
* Google Sheets
* Google Apps Script
* Cloudflare Pages

## Persyaratan

* Google Account
* Google Sheets
* Google Apps Script
* Cloudflare Pages 

---

## Struktur Spreadsheet

Buat sheet berikut:

### ORDERS_BEM
| ID | Waktu | Produk | Nama | Keterangan | Jumlah Tag | Daftar Tag | Total | Status |

### ORDERS_SEM
| ID | Waktu | Produk | Nama | Keterangan | Jumlah Tag | Daftar Tag | Total | Status |

### ORDERS_LEM
| ID | Waktu | Produk | Nama | Keterangan | Jumlah Tag | Daftar Tag | Total | Status |

### SETTINGS
| Produk | Nama Produk | Harga |
| ------ | ----------- | ----- |
| BEM    | BEM         | 750   |
| SEM    | SEM         | 350   |
| LEM    | LEM         | 250   |

---

## Instalasi

### 1. Google Spreadsheet

Buat spreadsheet baru lalu tambahkan seluruh sheet yang diperlukan.

### 2. Google Apps Script

Buat project Apps Script.

Tempel kode backend dan deploy sebagai:

Deployment → Web App

Pastikan akses:
Me

Who has access:
Anyone

Salin URL deployment.

---

### 3. Konfigurasi Website

Ganti URL Apps Script pada:

* index.html
* checkout.html
* admin.html

Contoh:

const API_URL = "URL_APPS_SCRIPT_ANDA";

---

### 4. Konfigurasi Admin

Ganti:

* Nomor WhatsApp Admin
* QRIS Pembayaran
* Nama Produk (opsional)
* Harga Produk (opsional)

---

### 5. Upload Website

Project dapat dijalankan menggunakan:

* Cloudflare Pages
* GitHub Pages
* Netlify
* Hosting HTML biasa

---
## Struktur Folder

```text
.
├── assets/
│   ├── css/
│   │   └── style.css
│   └── images/
│       ├── cover.png
│       ├── qris.jpg
│       ├── bem.webp
│       ├── sem.webp
│       ├── lem.webp
│       ├── whatsapp.svg.webp
│       └── ori.svg
├── index.html
├── checkout.html
├── payment.html
├── admin.html
└── README.md
```
---

## Catatan

Sebelum digunakan:

1. Ganti QRIS pada folder assets/images.
2. Ganti nomor WhatsApp Admin.
3. Ganti URL Apps Script.
4. Sesuaikan harga pada sheet SETTINGS.
5. Deploy ulang Apps Script setelah melakukan perubahan backend.

---

## Lisensi

Project ini dibagikan secara gratis untuk tujuan pembelajaran dan penggunaan pribadi.

Anda diperbolehkan:

* Menggunakan
* Memodifikasi
* Mengembangkan
* Membagikan ulang

dengan tetap mencantumkan kredit pembuat asli.

---

## Kredit

WARUNG_HAYDAY
https://www.facebook.com/yudha.cm

Dibuat untuk membantu komunitas Hay Day dalam mengelola pesanan secara lebih mudah menggunakan Google Sheets dan Google Apps Script.
