# UAS_PWL_A12202307026
GamerHub adalah platform penyewaan PlayStation dan game online yang memungkinkan pengguna menyewa konsol game dan judul game favorit mereka dengan mudah. Aplikasi ini dirancang untuk memberikan pengalaman yang cepat, aman, dan didukung penuh bagi para gamer.
Fitur Utama:

Penyewaan Game dan PlayStation:
Menyediakan koleksi game terbaru dan konsol PlayStation (PS2, PS3, PS4 Pro, PS5 Slim, PS5 Pro, PS VR2) untuk disewa.
Tampilan produk yang informatif dengan gambar, nama, deskripsi, dan harga sewa harian.
Fungsi "Add to Cart" untuk menambahkan produk ke keranjang belanja.
Manajemen Keranjang Belanja:
Menampilkan daftar item di keranjang dengan detail produk, jumlah, harga satuan, dan subtotal.
Kemampuan untuk memperbarui jumlah item atau menghapus item dari keranjang.
Perhitungan total harga sewa secara otomatis.
Proses Checkout:
Konfirmasi pesanan dengan ringkasan item dan total biaya.
Simulasi proses checkout yang mengarahkan ke halaman akun setelah konfirmasi.
Sistem Akun Pengguna:
Registrasi dan Login: Pengguna dapat membuat akun baru atau login ke akun yang sudah ada.
Manajemen Profil: Pengguna dapat memperbarui informasi pribadi seperti nama, nomor HP, alamat, dan mengubah password.
Pinjaman Aktif: Menampilkan daftar konsol atau game yang sedang disewa oleh pengguna, termasuk tanggal sewa dan rencana tanggal kembali.
Riwayat Transaksi: Menyimpan dan menampilkan riwayat transaksi penyewaan yang telah selesai.
Notifikasi Interaktif:
Sistem notifikasi dinamis (success/error) yang muncul di bagian atas halaman untuk memberikan umpan balik kepada pengguna (misalnya, "Item berhasil ditambahkan ke keranjang!", "Login gagal.").
Notifikasi otomatis hilang setelah beberapa detik atau dapat ditutup secara manual.
Desain Responsif:
Antarmuka pengguna yang dioptimalkan untuk berbagai ukuran layar, dari desktop hingga perangkat seluler, berkat penggunaan Bootstrap.

Teknologi yang Digunakan:

Frontend:
HTML5: Struktur dasar halaman web.
CSS3: Styling dan tata letak, termasuk penggunaan variabel CSS (:root), transisi (transition), dan animasi (@keyframes).
Bootstrap 5.3: Framework CSS untuk desain responsif dan komponen UI siap pakai (Navbar, Card, Modal, Form, Table, Button, dll.).
Font Awesome 6: Pustaka ikon untuk mempercantik tampilan.
Animate.css: Pustaka CSS untuk animasi tambahan (misalnya, efek bounce pada ikon keranjang).
JavaScript (Vanilla JS): Logika interaktif di sisi klien, termasuk:
Manajemen keranjang belanja (penambahan, pengurangan, penghapusan item).
Pemformatan mata uang Rupiah.
Fungsi notifikasi dinamis.
Interaksi AJAX dengan backend untuk fitur "Add to Cart".
Backend:
PHP: Bahasa pemrograman sisi server untuk memproses logika bisnis, interaksi database, dan manajemen sesi.
PDO (PHP Data Objects): Ekstensi PHP untuk mengakses database secara aman dan efisien.
Database:
MySQL (via gamerhub_db.sql): Sistem manajemen database relasional untuk menyimpan data pengguna, produk, sewa, dan detail sewa.
Server:
Apache/Nginx (asumsi): Web server untuk menjalankan aplikasi PHP.

Instruksi Instalasi/Jalankan Aplikasi:

Untuk menjalankan aplikasi GamerHub, Anda memerlukan lingkungan server web lokal (misalnya XAMPP, WAMP, Laragon) yang mendukung PHP dan MySQL.

1. Persiapan Lingkungan:

Instal XAMPP/WAMP/Laragon: Unduh dan instal salah satu paket server web lokal ini. Pastikan Apache dan MySQL berjalan.
2. Konfigurasi Database:

Buat Database:
Buka phpMyAdmin (biasanya di http://localhost/phpmyadmin).
Buat database baru dengan nama gamerhub_db.
Impor Skema Database:
Pilih database gamerhub_db yang baru Anda buat.
Klik tab "Import".
Pilih file MultipleFiles/gamerhub_db.sql dari direktori proyek Anda.
Klik "Go" untuk mengimpor skema tabel dan data awal (jika ada).
Konfigurasi Koneksi Database:
Buka file MultipleFiles/database.php.
Pastikan kredensial database sesuai dengan pengaturan MySQL Anda. Secara default, user adalah root dan pass adalah kosong ('').
3. Penempatan File Proyek:

Salin File Proyek:
Ekstrak atau salin semua file dan folder dari proyek ini (termasuk MultipleFiles/) ke dalam direktori htdocs (untuk XAMPP) atau www (untuk WAMP) atau public (untuk Laragon) di instalasi server web lokal Anda.

4. Jalankan Aplikasi:

Akses di Browser:
Buka browser web Anda.
Akses aplikasi melalui URL: http://localhost/gamerhub/ (ganti gamerhub dengan nama folder proyek Anda jika berbeda).
5. Penggunaan Aplikasi:

Anda dapat mulai menjelajahi koleksi game dan PlayStation.
Untuk menambahkan item ke keranjang atau mengakses fitur akun, Anda perlu mendaftar atau login terlebih dahulu melalui modal yang tersedia di navbar.
Setelah login, Anda bisa menambahkan item ke keranjang, melihat keranjang, melanjutkan ke checkout, dan mengelola profil Anda di halaman "Akun".
