# V_Universe
 
Selamat Datang di Website V Universe
Website ini adalah sebuah website fansite bagi penggemar Kim Taehyung, seorang penyanyi dan juga dancer dari Korea Selatan
Penggemar dapat mengirimkan pesan yang akan ditujukan kepada Kim Taehyung, dan dapat mengelola pesan yang dikirimkan

Dibuat oleh : Elsa Elisa Yohana  Sianturi
NIM : 12214013
Kelas : Pemrograman Web RA


Penjelasan : 
1. Client-side programing 
1.1 Manipulasi DOM dengan JavaScript
Pada kode yang diberikan, manipulasi DOM dilakukan dengan membuat formulir input menggunakan elemen <input>, di mana pengguna dapat mengisi data seperti nama, email, negara, tanggal lahir, pesan, dan rating. Data yang diinputkan oleh pengguna kemudian ditampilkan di dalam sebuah tabel HTML menggunakan JavaScript. Data yang diambil dari server atau yang telah diproses oleh PHP akan dimasukkan ke dalam tabel yang ada di halaman HTML, dan tampilan tabel ini akan diperbarui secara dinamis dengan menggunakan JavaScript. Ini memungkinkan tabel untuk menampilkan pesan-pesan yang telah dikirim, termasuk informasi terkait seperti nama pengirim, email, negara, dan rating.

1.2 Event Handling
Untuk menangani formulir input, terdapat 5 event berbeda yang digunakan dalam JavaScript. Event pertama adalah saat pengguna mengisi form dan mengirimkan data melalui tombol submit, JavaScript menangani event ini untuk memvalidasi input sebelum dikirimkan ke server. Validasi ini melibatkan pengecekan apakah semua field sudah terisi dengan benar dan apakah input seperti email dan rating valid. Selain itu, ada event untuk mengubah rating bintang, yang memungkinkan pengguna memberikan penilaian. Event lainnya termasuk ketika pengguna mengklik tombol untuk menghapus data atau menyimpan data ke dalam localStorage untuk menghindari kehilangan data jika halaman dimuat ulang. Semua event ini bertujuan untuk memastikan bahwa data yang dimasukkan pengguna telah divalidasi dengan benar dan tidak ada kesalahan sebelum diproses oleh PHP.

2. Server-Side Programing 

2.1 Pengelolaan Data dengan PHP
Pada bagian ini, data dari formulir dikirim menggunakan metode POST atau GET, lalu diproses di sisi server dengan PHP. Data yang diterima akan divalidasi terlebih dahulu untuk memastikan keabsahannya. Setelah validasi, data yang valid disimpan ke dalam basis data, termasuk informasi seperti jenis browser dan alamat IP pengguna untuk keperluan analisis atau pengelolaan.

2.2 Objek PHP Berbasis OOP
Pada bagian ini, digunakan konsep pemrograman berorientasi objek (OOP) untuk membuat objek PHP dengan empat metode. Metode-metode ini dapat menangani berbagai tugas, seperti validasi data, penyimpanan, pengambilan, dan penghapusan data dalam aplikasi, sehingga membuat pengelolaan kode menjadi lebih terstruktur dan mudah dikelola.

3. Database Management

3.1 Pembuatan Tabel Database
Pada bagian ini, dilakukan pembuatan database dengan perintah CREATE DATABASE, diikuti dengan pemilihan database yang baru dibuat menggunakan perintah USE. Selanjutnya, pembuatan tabel messages yang berisi beberapa kolom seperti id, name, email, country, birthdate, message, rating, browser, ip_address, dan created_at. Kolom-kolom ini memiliki tipe data yang sesuai dan beberapa di antaranya diberi atribut NOT NULL untuk memastikan data yang dimasukkan lengkap, serta kolom id sebagai primary key yang memiliki auto increment.

3.2 Konfigurasi Koneksi Database
Konfigurasi koneksi database mengacu pada pengaturan yang digunakan agar aplikasi dapat berkomunikasi dengan database yang telah dibuat. Biasanya, ini melibatkan pengaturan parameter seperti host, nama pengguna, kata sandi, dan nama database untuk memastikan koneksi yang sukses. Koneksi database ini dapat dilakukan menggunakan PHP dengan fungsi seperti mysqli_connect atau menggunakan framework tertentu.

3.3 Manipulasi Data pada Database
Manipulasi data pada database meliputi operasi untuk menyisipkan, mengubah, menghapus, dan mengambil data dari tabel. Setelah tabel dibuat, data yang diinput dari formulir akan disimpan menggunakan perintah INSERT INTO. Selain itu, data yang sudah ada dapat diubah atau dihapus dengan perintah UPDATE dan DELETE. Untuk mengambil data, perintah SELECT digunakan untuk mengakses dan menampilkan data yang dibutuhkan sesuai dengan kriteria yang ditentukan.

4. State Management 
4.1 State Management dengan Session
Session digunakan untuk menyimpan data sementara antar halaman. Fungsi session_start() memulai sesi di PHP yang memungkinkan data dapat disimpan di sisi server dan diakses di berbagai halaman selama sesi tersebut berlangsung.

Dalam kode ini, session_start() dipanggil di awal untuk memulai sesi, kemudian data terkait pengguna disimpan di dalam session:

Status pesan disimpan dalam session menggunakan $_SESSION['status'] yang akan menampilkan pesan status setelah proses tertentu selesai, lalu menghapusnya setelah ditampilkan.
Data form yang dimasukkan pengguna juga disimpan dalam session, misalnya $_SESSION['form_data'] untuk menampilkan kembali data form pada halaman setelah pengisian, jika terjadi kesalahan pengisian atau kesalahan lain.
Data ini hanya berlaku selama sesi pengguna tersebut aktif. Begitu sesi berakhir (misalnya browser ditutup), data ini akan hilang.

4.2 Pengelolaan State dengan Cookie dan Browser Storage
Cookie adalah cara untuk menyimpan data di sisi klien yang bertahan lebih lama daripada sesi. Cookie digunakan untuk menyimpan informasi pengguna yang akan diakses kembali di sesi-sesi berikutnya. Dalam kode ini, beberapa fungsi JavaScript digunakan untuk menetapkan, mengambil, dan menghapus cookie:

setCookie(name, value, days) digunakan untuk membuat cookie baru dengan nama dan nilai tertentu serta menetapkan waktu kadaluarsa.
getCookie(name) digunakan untuk mengambil nilai cookie berdasarkan nama.
deleteCookie(name) digunakan untuk menghapus cookie.
Dengan menggunakan cookie, data yang disimpan bisa bertahan lebih lama, bahkan ketika sesi atau browser ditutup.

Browser Storage adalah mekanisme penyimpanan data lokal pada browser yang lebih fleksibel. Ada dua jenis utama: Local Storage dan Session Storage. Local Storage menyimpan data tanpa kadaluarsa, sedangkan Session Storage menyimpan data hanya selama sesi browser. Dalam kode ini, browser storage digunakan untuk menyimpan data form:

saveToLocalStorage(key, value) menyimpan data ke dalam Local Storage.
getFromLocalStorage(key) mengambil data dari Local Storage.
removeFromLocalStorage(key) menghapus data dari Local Storage.
Dengan browser storage, data bisa disimpan di sisi klien tanpa melibatkan server dan dapat diakses kembali kapan saja.

Saya melakukan hal ini untuk index.php dan edit.php
