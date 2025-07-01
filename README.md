# CloudManager - Solusi Office Berbasis Cloud

Selamat datang di **CloudManager**, sebuah aplikasi office suite berbasis cloud yang lengkap dan dirancang sebagai platform *Software as a Service* (SaaS). Aplikasi ini menyediakan lingkungan kerja (workspace) yang terisolasi bagi setiap pengguna atau perusahaan, lengkap dengan dasbor admin super untuk manajemen sistem secara keseluruhan.

**Demo Langsung:** [https://cm.zyrex.win](https://cm.zyrex.win)

-----

## ✨ Fitur Utama

CloudManager hadir dengan serangkaian fitur untuk meningkatkan produktivitas dan manajemen bisnis:

  * **🏢 Manajemen Workspace:** Sistem multi-tenant di mana setiap pengguna atau perusahaan mendapatkan workspace-nya sendiri yang aman.
  * **👑 Dasbor Super Admin:** Panel kontrol terpusat untuk mengelola pengguna, workspace, paket langganan, dan pengaturan sistem secara keseluruhan.
  * **📄 Editor Dokumen:** Buat dan kelola dokumen teks kaya dengan editor WYSIWYG (What You See Is What You get) yang sudah terintegrasi.
  * **🗂️ Manajemen Aset Digital:** Unggah, simpan, dan kelola semua file dan media Anda di satu tempat.
  * **💰 Langganan & Penagihan:** Sistem langganan bawaan dengan dukungan untuk berbagai gateway pembayaran untuk mengelola paket dan transaksi.
  * **📅 Kalender & Acara:** Atur jadwal dan acara penting dengan fitur kalender yang intuitif.
  * \*\* Kontak & Buku Alamat:\*\* Kelola semua kontak bisnis dan personal Anda dengan mudah.
  * **🔗 Berbagi Cepat (Quick Share):** Bagikan dokumen dan file dengan aman kepada pihak eksternal dan lacak aksesnya.
  * **🔑 Manajemen Kunci API:** Buat dan kelola kunci API untuk integrasi dengan layanan lain.
  * **🌐 Halaman Landing & Blog:** Halaman depan yang dapat disesuaikan untuk memasarkan layanan SaaS Anda.
  * **🚀 Wizard Instalasi:** Proses instalasi yang mudah melalui antarmuka web.

-----

## 🛠️ Tumpukan Teknologi

Proyek ini dibangun menggunakan teknologi modern dan andal:

  * **Backend:** PHP 8+, Laravel 10
  * **Frontend:** Vite, Bootstrap 5, Sass
  * **Editor:** CKEditor 5
  * **Database:** MySQL

-----

## ⚙️ Instalasi

Untuk menjalankan proyek ini di lingkungan lokal Anda, ikuti langkah-langkah berikut.

### Prasyarat

  * PHP \>= 8.1
  * Composer
  * Node.js & NPM
  * Server Web (Nginx/Apache)
  * Database (misalnya MySQL)

### Langkah-langkah Instalasi

1.  **Clone repositori:**

    ```sh
    git clone https://github.com/jonathanzefanya/cloudmanager.git
    cd cloudmanager
    ```

2.  **Instal dependensi PHP:**

    ```sh
    composer install
    ```

3.  **Instal dependensi JavaScript:**

    ```sh
    npm install
    ```

4.  **Konfigurasi Lingkungan:**
    Salin file `.env.example` menjadi `.env`.

    ```sh
    cp .env.example .env
    ```

    Buka file `.env` dan konfigurasikan detail database Anda (DB\_HOST, DB\_PORT, DB\_DATABASE, DB\_USERNAME, DB\_PASSWORD).

5.  **Hasilkan Kunci Aplikasi:**

    ```sh
    php artisan key:generate
    ```

6.  **Buat Symbolic Link:**
    Untuk memastikan file yang diunggah dapat diakses secara publik.

    ```sh
    php artisan storage:link
    ```

7.  **Konfigurasi Web Server:**
    Arahkan *document root* server web Anda (misalnya, Nginx atau Apache) ke direktori `public/`.

8.  **Jalankan Wizard Instalasi:**
    Buka aplikasi di browser Anda. Anda akan secara otomatis diarahkan ke halaman `/install` untuk menyelesaikan proses pengaturan, termasuk membuat akun super admin pertama.

-----

## 🚀 Penggunaan

Aplikasi ini memiliki dua peran utama:

1.  **Super Admin:** Mengakses dasbor dari rute `/admin`. Super admin dapat mengelola seluruh aplikasi, termasuk:

      * Melihat statistik umum.
      * Mengelola pengguna dan workspace.
      * Membuat dan mengatur paket langganan.
      * Mengonfigurasi gateway pembayaran dan pengaturan sistem lainnya.

2.  **Pengguna Workspace (Kantor):** Mengakses dasbor dari rute `/office`. Pengguna dapat:

      * Membuat dan mengedit dokumen.
      * Mengunggah dan mengelola file.
      * Mengatur acara di kalender.
      * Mengelola kontak.
      * Berlangganan paket jika diperlukan.

-----

## 📄 Lisensi

Proyek CloudManager adalah perangkat lunak sumber terbuka yang dilisensikan di bawah [Lisensi MIT](https://opensource.org/licenses/MIT).