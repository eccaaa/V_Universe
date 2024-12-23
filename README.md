# V_Universe
 
Selamat Datang di Website V Universe
Website ini adalah sebuah website fansite bagi penggemar Kim Taehyung, seorang penyanyi dan juga dancer dari Korea Selatan
Penggemar dapat mengirimkan pesan yang akan ditujukan kepada Kim Taehyung, dan dapat mengelola pesan yang dikirimkan

Dibuat oleh : Elsa Elisa Yohana  Sianturi
NIM : 12214013
Kelas : Pemrograman Web RA

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

3.3Manipulasi Data
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
