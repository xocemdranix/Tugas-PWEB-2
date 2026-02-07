*<!DOCTYPE html>
<html lang="en">

<head>
    
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">*
Kode ini digunakan saat membuat kode html baru,menggunakan Bahasa inggris,menampilkan semua karakter dengan benar, dan membuat tampilan responsif di HP / tablet

*<title>my profile</title>*digunakan untuk membuat nama web itu sendiri.

*<link rel="stylesheet" href="style.css">
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
Kode ini digunakan untukm enghubungkan file CSS eksternal untuk styling, dan Memuat Font Awesome (library ikon)

*<div class="container">
Kode pembungkus utama seluruh konten

*<div class="profil">
Kode Bagian profil pengguna

*<img src="kid name finger.png" alt="foto profil">
Kode untuk menampilkan foto profil

*<h1 class="TimesNewRoman">Hi, I'm finger</h1>
Kode untuk menampilkan teks nama dan font yang dipakai

*<div class="social">
Kode bagian daftar sosial media

<h1 class="profil TimesNewRoman">MY SOCIALS</h1>
Kode budul section

*<a class="ig sosmed TimesNewRoman" href="...">
  <i class="fa-brands fa-instagram"></i> Instagram
etc
</a>
Kode untuk membuat link bisa dipencet dan memiliki symbol

*css
*{
    margin: 0;
    padding: 0;
}
Kode yang menghapus margin & padding bawaan browser dan agar layout mulai dari nol dan konsisten


*body{
    height: 100vh;
    width: 100%;
Kode untuk mengatur lebar dan tinggi full browser 

*background-image: url('nofire.jpeg');
background-position: center;
background-size: cover;
background-repeat: no-repeat;
Kode untuk menampilkan background gambar, membuat background dipusatkan, menutup seluruh layar, dan tidak diulang

*display: flex;
justify-content: center;
align-items: center;
Kode menggunakan Flexbox dan konten ditaruh tepat di tengah layar (horizontal + vertikal)

.profil{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 8px;
}
Kode membuat elemen profil disusun vertikal, semua rata tengah, dan ada jarak 8px antar elemen

.container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
Kode pembungkus semua konten, membuat susunan vertikal dan posisi ditengah

.profil img{
    width: 70px;
    height: 150px;
    border-radius: 50%;
}
Kode untuk mengatur ukuran gambar dan border-radius: 50% membuat gambar oval


.profil h1{
    color: white;
    padding: 5px;
    border-radius: 6px;
}
Kode membuat warna teks putih, adanya padding,dan sudut agak membulat

.TimesNewRoman {
    font-family: "Times New Roman", Times, serif;
    font-weight: 400;
    font-style: italic;
    font-size: 1.2rem;
    color: white;
}
Kode untuk Mengganti font ke Times New Roman, membuat tulisan italic, ukuran 1.2rem, dan warna putih
Class ini bisa dipasang ke elemen apa pun

.social{
    display: flex;
    flex-direction: column;
    gap: 12px;
    font-size: 0.5rem;
    justify-content: center;
}
Kode agar daftar tombol sosial disusun vertikal, jarak antar tombol 12px, dan ukuran teks kecil

Warna teks sosial
.social h1,
.social a{
    color: white;
}
Agar semua teks di section sosial jadi putih


.sosmed{
    background-color: rgb(17, 0, 255);
    width: 200px;
    height: 4vh;
Kode untuk mengatur warna tombol biru, lebar tetap, dan tinggi mengikuti tinggi layar

display: flex;
justify-content: center;
align-items: center;
Agar isi tombol rata tengah

position: relative;
border-radius: 6px;
padding: 4px;
Mengatur Sudut membulat,ada jarak dalam, dan relative dipakai supaya ikon bisa diposisikan

Ikon di dalam tombol
.sosmed i {
    position: absolute;
    left: 10px;
    font-size: 1.2rem;
}
Membuat ikon dipasang di kiri tombol dan tidak mengganggu teks tengah

Efek hover
.sosmed:hover{
    background-color: white;
    color: black;
    transition: 0.25
}
Agar saaat mouse diarahkan ke tombol: warna jadi putih + teks hitam