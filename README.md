# Mini Project 1 PBW
## Nama: Jabbar Hafizh Abdillah
## NIM: 2409116116

Website yang saya buat ini merupakan website portofolio yang berisikan penjelasan mengenai diri saya dari latar belakang, minat dan bakat, dan sertifikat yang telah saya raih. Adapun bahasa yang digunakan adalah HTML, CSS, Bootstrap 5.

# Tampilan Setiap Section/Fitur

## 1. Navbar

<img width="1899" height="80" alt="image" src="https://github.com/user-attachments/assets/86e325ec-5e67-4b53-a4ff-7e911a1304b0" />

Navbar pada website ini berada di bagian paling atas dan bersifat fixed sehingga tetap terlihat ketika pengguna melakukan scroll ke bawah. Tampilan navbar menggunakan warna gelap yang selaras dengan konsep dark mode pada keseluruhan website. Navbar pada website ini berada di bagian paling atas dan bersifat fixed sehingga tetap terlihat ketika pengguna melakukan scroll ke bawah. Tampilan navbar menggunakan warna gelap yang selaras dengan konsep dark mode pada keseluruhan website.

## 2. Home 

<img width="1898" height="796" alt="image" src="https://github.com/user-attachments/assets/19097683-dc04-4180-a235-da64ddf1931d" />

Pada bagian Home terdapat foto saya sendiri, kemudian terdapat perkenalan singkat yang memberitahu bahwa saya merupakan Mahasiswa Sistem Informasi Angkatan 2024.

## 3. About Me

<img width="1899" height="577" alt="image" src="https://github.com/user-attachments/assets/a6ea3c1e-d99b-40c5-832f-bb5d59f2b5c4" />

Selanjutnya, pada bagian About Me untuk tampilan informasinya disusun menggunakan komponen accordion dari Bootstrap sehingga setiap subbagian dapat dibuka dan ditutup sesuai kebutuhan pengguna. Adapun di About Me terdapat 3 hal penting yaitu:

### 1). Deskripsi Diri

<img width="1889" height="740" alt="image" src="https://github.com/user-attachments/assets/dcfa4e50-977b-477f-aea7-6e7115870fa8" />

Untuk bagian ini berisikan deskripsi diri saya, minat saya akan suatu hal, dan game yang saya minati

### 2). Skills

<img width="1897" height="783" alt="image" src="https://github.com/user-attachments/assets/91954b0c-961b-4bcb-bcab-d6799318dd82" />

Pada bagian ini terdapat progress bar yang menandakan seberapa paham saya akan suatu hal seperti bahasa pemrograman, pemahaman database, dan pemahaman jaringan komputer. Selain itu, saya juga menambahkan rank yang telah saya raih dalam game Valorant.

### 3). Pengalaman

<img width="1895" height="731" alt="image" src="https://github.com/user-attachments/assets/1a07ce93-9fc8-463d-bfbb-f45bb0446ff6" />

Dan terakhir, pada bagian ini merupakan list pengalaman saya dalam menjalankan organisasi ataupun kegiatan.

## 4. Certificates

<img width="1892" height="784" alt="image" src="https://github.com/user-attachments/assets/72a66efc-9d0b-4bbd-97da-bb6012d7586b" />

<img width="1888" height="771" alt="image" src="https://github.com/user-attachments/assets/1f70ab8b-be75-425a-9c2a-b8197d1159e3" />

Pada bagian ini, terdapat beberapa gambar sertifikat dari kegiatan atau pembelajaran yang telah saya raih. Saya menggunakan card agar gambar dapat ditaruh dan terdapat deskripsi singkat akan sertifikat tersebut, kemudian saya menggunakan layout grid 2x2 untuk 1 slide agar gambar tetap dapat terlihat dan memaksimalkan tampilan pada 1 slide tersebut. Dan juga terdapat tombol untuk pindah slide ke kiri ataupun ke kanan, bisa juga slide berpindah secara otomatis.

## 5. Footer

<img width="1897" height="41" alt="image" src="https://github.com/user-attachments/assets/682ad0cd-380c-4c1f-8da9-8924bdf475f7" />

Terakhir merupakan bagian Footer yang berisikan penanda bahwa saya yang membuat website tersebut.


# Penjelasan Code Setiap Section/Fitur

## 1. Navbar

Navbar dibuat menggunakan komponen navbar dari Bootstrap 5 dengan kelas `navbar-expand-lg`, yang berarti menu akan berubah menjadi hamburger menu pada layar kecil. Properti `fixed-top` digunakan agar navbar selalu berada di bagian atas layar saat pengguna melakukan scroll. Warna latar belakang diatur menggunakan kelas kustom `bg-dark-custom` yang didefinisikan di file CSS dengan warna `#111827` agar sesuai dengan konsep dark mode. Pergerakan indikator dikontrol menggunakan JavaScript melalui fungsi `moveIndicator()`, yang menghitung posisi link aktif menggunakan `getBoundingClientRect()` lalu mengatur properti width dan left secara dinamis.

## 2. Home

Hero section dibuat menggunakan elemen `<section id="home" class="hero-section">` dengan tinggi minimum `100vh` sehingga memenuhi satu layar penuh. Layout diatur menggunakan Flexbox melalui properti `display: flex, align-items: center, dan justify-content: center` agar konten berada tepat di tengah secara vertikal dan horizontal. Untuk source foto menggunakan `img src` yang terus dimasukkan ke dalam class `profile-img` untuk dimasukkan ke dalam CSS. Foto profil dibungkus dalam elemen `photo-frame` yang memiliki ukuran tetap.

## 3. About Me

Section About menggunakan komponen accordion dari Bootstrap yang memungkinkan konten dibuka dan ditutup secara dinamis tanpa perlu JavaScript tambahan. Setiap bagian seperti Deskripsi Diri, Skills, dan Pengalaman dibungkus dalam `accordion-item`. Tampilan accordion dimodifikasi menggunakan kelas `custom-accordion` pada CSS. Background bawaan Bootstrap dihilangkan dan diganti dengan tampilan transparan. Setiap subbab terdapat button `<button class="accordion-button">` untuk memicu efek buka-tutup.

## 4. Deskripsi Diri

Konten deskripsi ditempatkan di dalam `<div class="accordion-body">` yang berisi beberapa elemen `<p>`. Penggunaan paragraf terpisah bertujuan agar informasi lebih terstruktur dan mudah dibaca.

## 5. Skill dan Progress Bar

Skill ditampilkan menggunakan struktur kombinasi div dan komponen progress dari Bootstrap. Setiap skill memiliki container `skill-item` yang di dalamnya terdapat `skill-info` untuk menampilkan nama skill dan persentase secara sejajar menggunakan `display: flex` dan `justify-content: space-between`. Progress bar dibuat menggunakan `progress` sebagai container dan `progress-bar` sebagai isi yang akan menunjukkan persentase. Lebar progress ditentukan langsung pada CSS melalui kelas khusus seperti `htmlcssjs-bar`, `designdatabase-bar`, `python-bar`, dan `network-bar`, masing-masing dengan properti width sesuai persentase serta background berupa gradient warna berbeda agar terlihat lebih menarik. Yang terakhir pada bagian Valorant, terdapat class yang mengatur setiap gambar logo rank yaitu, `valorant-ranks`  yang menggunakan `position: relative` sehingga ikon rank dapat diposisikan secara absolut.

## 6. Pengalaman

Di dalam bagian ini, daftar pengalaman ditampilkan menggunakan elemen `<ul>` dan `<li>` untuk menjaga struktur informasi tetap rapi dan terorganisir. Setiap pengalaman dituliskan dalam satu baris list agar mudah dibaca serta memberikan kesan sistematis.

## 7. Certificates

Section Certificates menggunakan komponen `carousel` dari Bootstrap untuk memungkinkan pergeseran slide secara otomatis maupun manual. Elemen utama `div` dengan kelas `carousel slide` memiliki atribut `data-bs-ride="carousel"` yang mengaktifkan fitur auto-slide. Di dalam setiap `carousel-item`, sertifikat ditampilkan menggunakan layout grid berbasis CSS Grid melalui kelas `certificate-grid`. Properti `grid-template-columns: repeat(2, 1fr)` membuat layout menjadi dua kolom, sehingga setiap slide menampilkan empat card dalam susunan 2x2.

## 8. Footer

Footer dibuat sederhana menggunakan elemen `<footer>` dengan kelas `bg-dark-custom` agar konsisten dengan warna navbar. Teks diberi warna putih dan ditata di tengah menggunakan kelas Bootstrap `text-center`. Padding `vertikal` ditambahkan menggunakan `py-3` untuk memberikan ruang yang cukup agar footer tidak terlihat terlalu sempit.


# Tekhnologi yang Digunakan

- HTML
- CSS
- JavaScript
- Bootstrap 5



