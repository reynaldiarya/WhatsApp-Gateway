# WhatsApp Gateway Workshop

WhatsApp Gateway Workshop adalah proyek berbasis web untuk apotek yang memungkinkan pencatatan pesan antara pelanggan dan pegawai apotek. Proyek ini dikembangkan dengan framework **Laravel**, ditujukan sebagai studi kasus untuk mata kuliah Pengembangan Perangkat Lunak Wokrshop.

## Fitur Utama
- **Pencatatan Pesan WhatsApp**: Catat pesan antara pelanggan dan pegawai apotek untuk kemudahan administrasi.
- **Integrasi dengan Fonnte API**: Memanfaatkan API Fonnte untuk mencatat komunikasi WhatsApp.
- **Dashboard Responsif**: Antarmuka pengguna berbasis Bootstrap yang mendukung desktop dan perangkat mobile.
- **Manajemen Data Pelanggan**: Tambah, edit, dan hapus data pelanggan.
- **Histori Komunikasi**: Pantau dan arsipkan pesan yang dikirimkan.

## Persyaratan Sistem
- **PHP** versi 8.1 atau lebih baru
- **Composer** versi terbaru
- **MySQL** atau database lain yang kompatibel
- **Laravel** versi 10.x

## Instalasi

### 1. Clone Repository
```bash
git clone https://github.com/reynaldiarya/WhatsApp-Gateway-Workshop.git
cd WhatsApp-Gateway-Workshop
```

### 2. Instal Dependensi
Jalankan perintah berikut untuk menginstal semua dependensi backend:
```bash
composer install
```

### 3. Konfigurasi Lingkungan
Salin file `.env.example` menjadi `.env` dan atur konfigurasi yang sesuai:
```bash
cp .env.example .env
```
Edit file `.env` untuk mengatur:
- Database (DB_DATABASE, DB_USERNAME, DB_PASSWORD)
- App Key (`php artisan key:generate` untuk menghasilkan kunci aplikasi)

### 4. Migrasi Database
Jalankan migrasi untuk membuat tabel database:
```bash
php artisan migrate
```

### 5. Jalankan Server Lokal
Gunakan perintah berikut untuk menjalankan server lokal:
```bash
php artisan serve
```
Akses aplikasi di: `http://localhost:8000`

### 6. Update API Key
Pastikan API Key Fonnte sudah diatur dengan benar pada menu setting `Token Fonnte`. Contoh pengaturan:
```
Token Fonnte = tokenanda
```

### Integrasi API Fonnte
Proyek ini menggunakan layanan Fonnte untuk mencatat komunikasi WhatsApp. Pastikan Anda memiliki API Key dari Fonnte dan mengaturnya di setting.

## Lisensi
Proyek ini menggunakan lisensi [MIT](LICENSE).
