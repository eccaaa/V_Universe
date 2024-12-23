# V_Universe
 
Selamat Datang di Website V Universe
Website ini adalah sebuah website fansite bagi penggemar Kim Taehyung, seorang penyanyi dan juga dancer dari Korea Selatan
Penggemar dapat mengirimkan pesan yang akan ditujukan kepada Kim Taehyung, dan dapat mengelola pesan yang dikirimkan

Dibuat oleh 
# Elsa Elisa Yohana  Sianturi
# NIM : 12214013
# Kelas : Pemrograman Web RA

   
# Tentang Proyek
Website ini dirancang untuk mengelola pesan dukungan kepada Kim Taehyung. Pengguna dapat:

Mengisi formulir dengan nama, email, negara, tanggal lahir, pesan, dan rating.
Menampilkan data yang dimasukkan dalam tabel dinamis.
Melakukan operasi CRUD (Create, Read, Update, Delete).
Website ini menggunakan kombinasi teknologi client-side dan server-side untuk memastikan pengalaman pengguna yang interaktif dan data yang terkelola dengan baik.

# Fitur Utama

# 1. Client-Side Programming
1.1 Manipulasi DOM dengan JavaScript
Membuat formulir input interaktif.
Menampilkan data pengguna secara dinamis ke dalam tabel HTML.

1.2 Event Handling
Validasi formulir saat pengguna mengirim data.
Penanganan tombol submit, hapus, dan perubahan rating bintang.
Menyimpan data sementara di localStorage agar tidak hilang saat reload halaman.

# 2. Server-Side Programming
2.1 Pengelolaan Data dengan PHP
Data dikirim menggunakan metode POST atau GET.
Validasi data untuk memastikan input lengkap dan valid.
Data yang valid disimpan ke database, termasuk metadata seperti alamat IP dan jenis browser.

2.2 OOP dengan PHP
Menggunakan pendekatan Object-Oriented Programming (OOP) untuk pengelolaan kode.
Metode meliputi validasi, penyimpanan, pengambilan, dan penghapusan data.

# 3. Database Management
3.1 Pembuatan Database
Tabel messages memiliki kolom seperti id, name, email, country, birthdate, message, rating, dll.

3.2 Koneksi Database
Konfigurasi parameter database untuk komunikasi dengan aplikasi.

3.3 Manipulasi Data
Menyisipkan data dengan INSERT INTO.
Mengubah data dengan UPDATE.
Menghapus data dengan DELETE.
Mengambil data dengan SELECT untuk ditampilkan ke tabel.

# 4. State Management
4.1 Session
Menyimpan status pesan sementara, seperti data form atau pesan konfirmasi.

4.2 Cookie & Browser Storage
Cookie: Menyimpan data pengguna untuk sesi yang lebih lama.
Local Storage: Menyimpan data form agar tetap ada meskipun halaman dimuat ulang.



# Langkah Langkah Hosting Dengan Infinityfree
1. Persiapkan File dan Folder
Saya memastikan semua file website saya sudah lengkap, termasuk config.php, edit.php, onboarding.html, index.php, message.php, process.php, serta folder image dan style. 

2. Daftar dan Login ke InfinityFree
Saya mendaftar di InfinityFree. Setelah berhasil mendaftar, saya langsung login ke dashboard InfinityFree untuk memulai proses hosting.

3. Membuat Akun Hosting
Saya membuat akun hosting baru dengan memilih opsi Create Account. Lalu, saya memilih domain subdomain dan mengetikkan nama v-universe sehingga domain saya menjadi v-universe.infinityfreeapp.com. Setelah itu, saya menyelesaikan proses dengan menekan tombol Create Account.

4. Membuat Database di InfinityFree
Saya membuka menu MySQL Databases di dashboard InfinityFree.
Saya membuat database baru dengan mengisi nama database, username, dan password sesuai petunjuk di form tersebut. 
Setelah itu, saya mencatat semua detail ini karena akan digunakan di file config.php.

6. Mengunggah File ke File Manager
Saya membuka File Manager di dashboard InfinityFree.
Saya masuk ke folder htdocs, yang merupakan folder root untuk website saya.
Saya mengunggah file seluruh file saya  yang telah  dipersiapkan tadi ke dalam folder htdocs menggunakan fitur upload.


7. Menyesuaikan File config.php
Saya membuka file config.php di editor bawaan File Manager.
Saya menyesuaikan pengaturan koneksi database dengan informasi dari InfinityFree 

website saya telah di hosting, dengan link http://v-universe.infinityfreeapp.com/onboarding.html
Tetapi karena website hosting ini gratis, maka link nya akan dapat di akses setelah 72 jam deploy

# Layanan Penyedia Hosting Web yang Cocok : Hostinger 

Hostinger adalah pilihan ideal untuk hosting karena menawarkan performa tinggi dengan harga terjangkau. Dengan pusat data yang tersebar di berbagai lokasi, termasuk Asia, website Anda dapat diakses dengan cepat, terutama oleh audiens di wilayah tersebut. Panel kontrol hPanel yang intuitif memudahkan pengelolaan hosting, bahkan untuk pemula. Selain itu, Hostinger menyediakan fitur keamanan lengkap, seperti SSL gratis, proteksi DDoS, dan backup otomatis, untuk menjaga data pengguna tetap aman.

Layanan Hostinger juga didukung teknologi modern seperti PHP 8.0, MySQL, dan LiteSpeed Cache untuk memastikan performa optimal. Dengan dukungan pelanggan 24/7 yang responsif, Anda tidak perlu khawatir jika mengalami kendala teknis. Hostinger bahkan menawarkan garansi uang kembali 30 hari, sehingga Anda dapat mencoba layanannya tanpa risiko. Kombinasi fitur ini membuat Hostinger cocok untuk proyek Anda yang membutuhkan hosting andal dan efisien.

# Memastikan keamanan data
Website ini menggunakan teknik pengelolaan sesi yang aman dan perlindungan cookie untuk mencegah akses ilegal atau manipulasi data.

# Konfigurasi  Server

**Konfigurasi Dasar Server:**  
File `config.php` mendefinisikan pengaturan inti untuk koneksi server database, seperti nama host, nama pengguna, kata sandi, dan nama database. File ini memastikan bahwa aplikasi PHP dapat terhubung dengan database yang dituju untuk menjalankan berbagai operasi seperti menyimpan atau mengambil data. Konfigurasi ini biasanya memanfaatkan PDO (PHP Data Objects) untuk membangun koneksi yang aman, efisien, dan mendukung fitur-fitur modern seperti pernyataan yang disiapkan (prepared statements). Selain itu, file ini sering digunakan untuk menyimpan variabel global, seperti parameter server, yang dapat diakses oleh file lain di seluruh aplikasi, memastikan konsistensi dan mempermudah pengelolaan pengaturan server.

**Proses dan Interaksi Server:**  
File `process.php` berfungsi sebagai penghubung antara logika aplikasi dan database server. File ini menangani operasi penting seperti pengolahan data yang dikirim melalui formulir menggunakan metode POST atau GET, validasi data pengguna, serta eksekusi kueri SQL untuk berbagai operasi database. `process.php` memanfaatkan konfigurasi yang diatur dalam `config.php` untuk memastikan koneksi database tetap aman dan stabil, dengan menggunakan prepared statements untuk mencegah ancaman seperti SQL Injection. Selain itu, file `index.php` bertindak sebagai antarmuka utama aplikasi, yang bertanggung jawab untuk memuat formulir atau data yang ditampilkan kepada pengguna.

**Pengelolaan Pesan pada Server:**  
Proses pengelolaan data pesan dilakukan melalui class `Message`, yang berfungsi sebagai abstraksi dari berbagai operasi database untuk pesan. Class ini mendukung operasi CRUD (Create, Read, Update, Delete) dan memastikan keamanan melalui pembersihan data serta prepared statements. Data yang dikirimkan oleh pengguna, seperti nama, email, pesan, dan detail lainnya, diolah di server, divalidasi, dan disimpan di tabel `messages` di database. Class ini juga menyediakan fitur tambahan seperti pengecekan keberadaan pesan dengan ID tertentu (`exists`) dan pembersihan data menggunakan metode `cleanData`, sehingga server dapat menangani interaksi data dengan lebih aman dan andal. Kombinasi ini menjamin efisiensi pengelolaan server serta pengalaman pengguna yang mulus.
