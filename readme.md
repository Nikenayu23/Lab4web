
# Lab4Web PRAKTIKUM 3-PEMROGRAMAN WEB (CSS LAYOUT) 
NIKEN AYU RISTIANI
T1.23.C1
312310026
Modul Praktikum pemograman Lab4Web

## PRAKTIKUM 3 

## Modul Praktikum Pemograman Web

membuat box element
Element HTML dapat dianggap sebagai sebuah Box atau kotak. Box tersebut digunakan untuk
membuat layout web. Pada dasarnya semua element HTML adalah box dengan beberapa perbedaan.
Ada yang floating ada juga yang tanpa floating.
Tag yang biasanya digunakan dalam merancang layout web adalah tag div dengan konsep box
element. Konsep box element terdiri dari Margin, Border, Padding, dan Content.

CSS Float Property

CSS Float Property memungkinkan elemen HTML dibuat seolah-olah mengambang diantara
elemen yang lainnya. Dengan konsep tersebut dapat dengan mudah menentukan posisi atau letak
sebuah elemen HTML. Sehingga dalam membuat layout web dapat dengan mudah dilakukan.
Property yang digunakan untuk mendefinisikan adalah float dan clear.
```bash
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Box Element</title>
</head>
<body>
<header>
<h1>Box Element</h1>
</header>
</body>
</html>

Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut. 

<section>
<div class="div1">Div 1</div>
<div class="div2">Div 2</div>
<div class="div3">Div 3</div>
</section>

```
kemudian buka browser untuk melihat hasilnya seperti berikut.
## Box Element

![App Screenshot](./image%20lab4web/3.png)

## Penambahan div 4

![App Screenshot](./image%20lab4web/2.png)

## STYLE CSS

```bash
<style>
div {
float:left;
padding: 10px;
} 
.div1 {
background: red;
}
.div2 {
background: yellow;
}
.div3 {
background: green;
}
.div4 {
background-color: blue;
clear: left;
float: none;
}
</style>
```

mengatur Clearfix Element 

```bash
<section>
<div class="div1">Div 1</div>
<div class="div2">Div 2</div>
<div class="div3">Div 3</div>
<div class="div4">Div 4</div>
</section>
```
Membuat Layout Sederhana 
## Layout sederhana

![App Screenshot](./image%20lab4web/5.jpeg)

```bash
  <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Layout Sederhana</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<div id="container">
</div>
</body>
</html>

<header>
<h1>Layout Sederhana</h1>
</header>
<nav>
<a href="home.html" class="active">Home</a>
<a href="artikel.html">Artikel</a>
<a href="about.html">About</a>
<a href="kontak.html">Kontak</a>
</nav>
<section id="hero"></section>
<section id="wrapper">
<section id="main"></section>
<aside id="sidebar"></aside>
</section>
<footer>
<p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

## Kerangka Layout

![App Screenshot](./image%20lab4web/8.png)



## tampilan sederhana

![App Screenshot](./image%20lab4web/6.png)



```bash
<aside id="sidebar">
<div class="widget-box">
<h3 class="title">Widget Header</h3>
<ul>
<li><a href="#">Widget Link</a></li>
<li><a href="#">Widget Link</a></li>
<li><a href="#">Widget Link</a></li>
<li><a href="#">Widget Link</a></li>
<li><a href="#">Widget Link</a></li>
</ul>
</div>
<div class="widget-box">
<h3 class="title">Widget Text</h3>
<p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
pharetra est nunc, nec pretium nunc pretium ac.</p>
</div>
</aside>
```
```bash
<section id="main">
<div class="row">
<div class="box">
<img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
<h3>Heading</h3>
<p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
<a href="#" class="btn btn-default">View detail</a>
</div>
<div class="box">
<img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
class="image-circle">
<h3>Heading</h3>
<p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
<a href="#" class="btn btn-default">View detail</a>
</div>
<div class="box">
<img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
<h3>Heading</h3>
<p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
<a href="#" class="btn btn-default">View detail</a>
</div>
</div>
</section>
```
```bash
<hr class="divider" />
<article class="entry">
<h2>First featurette heading.</h2>
<img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
<h2>First featurette heading.</h2>
<img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
```

## CSS

tambahkan kode CSS untuk membuat layoutnya

```bash
  /* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400
;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0
,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
margin: 0;
padding: 0;
}
body {
line-height:1;
font-size:100%;
font-family:'Open Sans', sans-serif;
color:#5a5a5a;
}
#container {
width: 980px;
margin: 0 auto;
box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
padding: 20px;
}
header h1 {
margin: 20px 10px;
```
```bash
  /* navigasi */
nav {
display: block;
background-color: #1f5faa;
}
nav a {
padding: 15px 30px;
display: inline-block;
color: #ffffff;
font-size: 14px;
text-decoration: none;
font-weight: bold;
}
nav a.active,
nav a:hover {
background-color: #2b83ea;
}
```

## Halaman awal

![App Screenshot](./image%20lab4web/11.png)


```bash
 <section id="hero">
<h1>Hello World!</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
<a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
## Hero Panel , Hello World

![App Screenshot](./image%20lab4web/12.png)


```bash
  /* Hero Panel */
#hero {
background-color: #e4e4e5;
padding: 50px 20px;
margin-bottom: 20px;
}
#hero h1 {
margin-bottom: 20px;
font-size: 35px;
}
#hero p {
margin-bottom: 20px;
font-size: 18px;
line-height: 25px;
}
#main {
float: left;
width: 640px;
padding: 20px;
}
/* sidebar area */
#sidebar {
float: left;
width: 260px;
padding: 20px;
}
```
```bash
  /* main content */
#wrapper {
margin: 0;
}
#main {
float: left;
width: 640px;
padding: 20px;
}
/* sidebar area */
#sidebar {
float: left;
width: 260px;
padding: 20px;
}

```

```bash
  /* widget */
.widget-box {
border:1px solid #eee;
margin-bottom:20px;
}
.widget-box .title {
padding:10px 16px;
background-color:#428bca;
color:#fff;
}
.widget-box ul {
list-style-type:none;
}
.widget-box li {
border-bottom:1px solid #eee;
}
.widget-box li a {
padding:10px 16px;
color:#333;
display:block;
text-decoration:none;
}
.widget-box li:hover a {
background-color:#eee;
}
.widget-box p {
padding:15px;
line-height:25px;
}
```
## Tampilan Sidebar Widget

![App Screenshot](./image%20lab4web/14.png)

```bash
  /* footer */
footer {
clear:both;
background-color:#1d1d1d;
padding:20px;
color:#eee;
}
```
```bash
/* box */
.box {
display:block;
float:left;
width:33.333333%;
box-sizing:border-box;
-moz-box-sizing:border-box;
-webkit-box-sizing:border-box;
padding:0 10px;
text-align:center;
}
.box h3 {
margin: 15px 0;
}
.box p {
line-height: 20px;
font-size: 14px;
margin-bottom: 15px;
}
box img {
border: 0;
vertical-align: middle;
}
.image-circle {
border-radius: 50%;
}
.row {
margin: 0 -10px;
box-sizing: border-box;
-moz-box-sizing: border-box;
-webkit-box-sizing: border-box;
}
.row:after, .row:before,
.entry:after, .entry:before {
content:'';
display:table;
}
.row:after,
.entry:after {
clear:both;
}
```
## Tampilan Content

![App Screenshot](./image%20lab4web/13.png)


```bash
.divider {
border:0;
border-top:1px solid #eeeeee;
margin:40px 0;
}
/* entry */
.entry {
margin: 15px 0;
}
.entry h2 {
margin-bottom: 20px;
}
.entry p {
line-height: 25px;
}
.entry img {
float: left;
border-radius: 5px;
margin-right: 15px;
}
.entry .right-img {
float: right;
}
```

## Tampilan artikel

![App Screenshot](./image%20lab4web/15.png)


![App Screenshot](./image%20lab4web/18.png)


## Membuat Layout Contact me

```bash
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Contact Me</h1>
        </header>
        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>
        <!-- service -->
	<section class="service">
		<div class="container">
			<h3>CONTACT INFO : MIRANDA</h3>
			<div class="box">
				<div class="col-4">
					<h4>Address :</h4>
					<p>Cikarang Selatan,Kab.BEKASI</p>
				</div>
				<div class="col-4">
					<h4>Email :</h4>
					<p>mirandasiagian198@gmail.com</p>
				</div>
				<div class="col-4">
					<h4>Hp :</h4>
					<p>081366083182</p>
				</div>
			</div>
        <section id="kontak">
            <div class="login">
                <input type="text" placeholder="Your Name" class="input">
                <input type="text" placeholder="Your Email Address" class="input">
            </div>

            <div class="subject">
                <input type="text" placeholder="Subject" class="input">
            </div>

            <div class="msg">
                <textarea cols="35" rows="10" class="area" placeholder="Your Message" class="input"></textarea>
            </div>

            <button type="submit"> Send </button>

        </section>
        <footer>
            <p>&copy; 2021 - Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```

## Tampilan Contact Me

![App Screenshot](./image%20lab4web/1.png)



## Membuat Layout About 
```bash
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1-0">
	<title>about me</title>
	<link rel="stylesheet" href="style.css">
</head>
<body>
	<div id="container">
		<header>
			<h1>about me</h1>
		</header>
		<nav>
			<a href="home.html" class="active">home</a>
			<a href="artikel.html">artikel</a>
			<a href="about.html">about</a>
			<a href="kontak.html">kontak</a>
		</nav>
		<section id="introduce">
			<div class="row">
				<img src="nizar.jpg" title="miranda oktavia" alt="miranda oktavia" class="image-circle" width="230"style="float: left; border: 2px solid black;">
				<h1>hello!</h1>
				<p> nama saya miranda oktavia. saya adalah seorang mahasiswi dari <i>universitas pelita bangsa</i> yang saat ini sedang mempelajari materi layout CSS dalam mata kuliah <i>pemrograman web</i>.</p>
			</div>
		</section>
	</div>
</body>
</html>

```
## Tampilan About

![App Screenshot](./image%20lab4web/7.png)


## PRAKTIKUM 4 

Konfigurasi koneksi database

Selanjutnya membuat konfigurasi untuk menghubungkan dengan database server. Konfigurasi
dapat dilakukan dengan du acara, yaitu pada file app/config/database.php atau menggunakan
file .env. Pada praktikum ini kita gunakan konfigurasi pada file .env.

![App Screenshot](./image/pra5.png)

 Membuat Model

Selanjutnya adalah membuat Model untuk memproses data Artikel. Buat file baru pada
direktori app/Models dengan nama ArtikelModel.php

![App Screenshot](./image/pra4.png)

 Membuat Controller

Buat Controller baru dengan nama Artikel.php pada direktori app/Controllers.

![App Screenshot](./image/pra6.png)

 Membuat View

Buat direktori baru dengan nama artikel pada direktori app/views, kemudian buat file baru
dengan nama index.php.

![App Screenshot](./image/pra7.png)

![App Screenshot](./image/pra10.png)

Selanjutnya buka browser kembali, dengan mengakses url http://localhost:8080/artikel

![App Screenshot](./image/pra8.png)

 Membuat Tampilan Detail Artikel

Tampilan pada saat judul berita di klik maka akan diarahkan ke halaman yang berbeda.
Tambahkan fungsi baru pada Controller Artikel dengan nama view().

![App Screenshot](./image/pra9.png)

 Membuat View Detail

Buat view baru untuk halaman detail dengan nama app/views/artikel/detail.php.

![App Screenshot](./image/pra10.png)

Membuat Routing untuk artikel detail

Buka Kembali file app/config/Routes.php, kemudian tambahkan routing untuk artikel detail.

![App Screenshot](./image/pra11.png)

 Membuat Menu Admin

Menu admin adalah untuk proses CRUD data artikel. Buat method baru pada Controller
Artikel dengan nama admin_index().

![App Screenshot](./image/pra13.png)

Akses menu admin dengan url http://localhost:8080/admin/artikel

![App Screenshot](./image/pra14.png)

Menambah Data Artikel
Tambahkan fungsi/method baru pada Controller Artikel dengan nama add().

![App Screenshot](./image/pra15.png)

Kemudian buat view untuk form tambah dengan nama form_add.php

![App Screenshot](./image/pra16.png)

![App Screenshot](./image/pra17.png)

![App Screenshot](./image/pra18.png)

Kemudian buat view untuk form tambah dengan nama form_edit.php

![App Screenshot](./image/pra19.png)

![App Screenshot](./image/pra20.png)

 Menghapus Data

Tambahkan fungsi/method baru pada Controller Artikel dengan nama delete().

![App Screenshot](./image/pra21.png)

## PRAKTIKUM 5

Membuat Layout Utama

Buat folder layout di dalam app/Views/
Buat file main.php di dalam folder layout dengan kode berikut:

![App Screenshot](./image/pra22.png)

Modifikasi File View

Ubah app/Views/home.php agar sesuai dengan layout baru:

![App Screenshot](./image/pra23.png)

Sesuaikan juga untuk halaman lainnya yang ingin menggunakan format layout yang baru.

Menampilkan Data Dinamis dengan View Cell

View Cell adalah fitur yang memungkinkan pemanggilan tampilan dalam bentuk komponen
yang dapat digunakan ulang. Cocok digunakan untuk elemen-elemen yang sering muncul di
berbagai halaman seperti sidebar, widget, atau menu navigasi.

![App Screenshot](./image/pra24.png)

Membuat Class View Cell

Buat folder Cells di dalam app/
Buat file ArtikelTerkini.php di dalam app/Cells/ dengan kode berikut:

![App Screenshot](./image/pra25.png)

Membuat View untuk View Cell

Buat folder components di dalam app/Views/
Buat file artikel_terkini.php di dalam app/Views/components/ dengan kode berikut:

![App Screenshot](./image/pra26.png)

## PRAKTIKUM 6

Membuat Model User

Selanjutnya adalah membuat Model untuk memproses data Login. Buat file baru pada direktori
app/Models dengan nama UserModel.php

![App Screenshot](./image/pra26b.png)

Membuat Controller User

Buat Controller baru dengan nama User.php pada direktori app/Controllers. Kemudian
tambahkan method index() untuk menampilkan daftar user, dan method login() untuk proses
login.

![App Screenshot](./image/pra26c.png)

Membuat Database Seeder

Database seeder digunakan untuk membuat data dummy. Untuk keperluan ujicoba modul
login, kita perlu memasukkan data user dan password kedaalam database. Untuk itu buat
database seeder untuk tabel user. Buka CLI, kemudian tulis perintah berikut:

php spark make:seeder UserSeeder

Selanjutnya, buka file UserSeeder.php yang berada di lokasi direktori

/app/Database/Seeds/UserSeeder.php kemudian isi dengan kode berikut:

![App Screenshot](./image/pra26d.png)

Selanjutnya buka kembali CLI dan ketik perintah berikut:

php spark db:seed UserSeeder

![App Screenshot](./image/pra26e.png)

Uji Coba Login

Selanjutnya buka url http://localhost:8080/user/login seperti berikut:

![App Screenshot](./image/pra26.png)

Menambahkan Auth Filter

Selanjutnya membuat filer untuk halaman admin. Buat file baru dengan nama Auth.php pada
direktori app/Filters.

![App Screenshot](./image/pra27b.png)

Selanjutnya buka file app/Config/Filters.php tambahkan kode berikut:

'auth' => App\Filters\Auth::class

Selanjutnya buka file app/Config/Routes.php dan sesuaikan kodenya.

![App Screenshot](./image/pra27c.png)

Percobaan Akses Menu Admin

Buka url dengan alamat http://localhost:8080/admin/artikel ketika alamat tersebut diakses
maka, akan dimuculkan halaman login.

![App Screenshot](./image/pra26.png)

Fungsi Logout

Tambahkan method logout pada Controller User seperti berikut:

```bash
public function logout()
{
  session()->destroy();
return redirect()->to('/user/login');
}
```

Membuat Pagination

Pagination merupakan proses yang digunakan untuk membatasi tampilan yang panjang
dari data yang banyak pada sebuah website. Fungsi pagination adalah memecah tampilan
menjadi beberapa halaman tergantung banyaknya data yang akan ditampilkan pada
setiap halaman.

Pada Codeigniter 4, fungsi pagination sudah tersedia pada Library sehingga cukup mudah
menggunakannya.
Untuk membuat pagination, buka Kembali Controller Artikel, kemudian modifikasi kode
pada method admin_index seperti berikut.

![App Screenshot](./image/acc3.png)

Kemudian buka file views/artikel/admin_index.php dan tambahkan kode berikut

dibawah deklarasi tabel data.

<?= $pager->links(); ?>

Selanjutnya buka kembali menu daftar artikel, tambahkan data lagi untuk melihat
hasilnya.

![App Screenshot](./image/pra27.png)

Membuat Pencarian

Pencarian data digunakan untuk memfilter data.
Untuk membuat pencarian data, buka kembali Controller Artikel, pada method

admin_index ubah kodenya seperti berikut:

![App Screenshot](./image/acc3a.png)

Kemudian buka kembali file views/artikel/admin_index.php dan tambahkan form

pencarian sebelum deklarasi tabel seperti berikut:

![App Screenshot](./image/acc3a.png)

Dan pada link pager ubah seperti berikut.

<?= $pager->only(['q'])->links(); ?>

Selanjutnya ujicoba dengan membuka kembali halaman admin artikel, masukkan kata
kunci tertentu pada form pencarian.

![App Screenshot](./image/acc2.png)

## PRAKTIKUM 7 

Upload Gambar pada Artikel

Menambahkan fungsi unggah gambar pada tambah artikel.
Buka kembali Controller Artikel pada project sebelumnya, sesuaikan kode pada method add seperti berikut:

![App Screenshot](./image/tikum7.png)

Kemudian pada file views/artikel/form_add.php tambahkan field input file seperti
berikut.

```bash
<p>
<input type="file" name="gambar">
</p>
```

Dan sesuaikan tag form dengan menambahkan ecrypt type seperti berikut.

```bash
<form action="" method="post" enctype="multipart/form-data">
```

Ujicoba file upload dengan mengakses menu tambah artikel.

```bash
![App Screenshot](./image/pra17.png)
```

## PRAKTIKUM 9

Membuat Model Kategori

Buat file model baru di `app/Models` dengan nama `KategoriModel.php`:

![App Screenshot](./lab7web/image/praktikum9/A.png)

Memodifikasi Model Artikel

Modifikasi `ArtikelModel.php` untuk mendefinisikan relasi dengan `KategoriModel`:

![App Screenshot](./lab7web/image/praktikum9/B.png)

Menambahkan method `getArtikelDenganKategori()` untuk mengambil data artikel beserta
nama kategorinya menggunakan join.

Memodifikasi Controller Artikel

Modifikasi `Artikel.php` untuk menggunakan model baru dan menampilkan data relasi:

![App Screenshot](./lab7web/image/praktikum9/C.png)

Memodifikasi View

Buka folder view/artikel sesuaikan masing-masing view.
index.php

![App Screenshot](./lab7web/image/praktikum9/D.png)

admin_index.php

![App Screenshot](./lab7web/image/praktikum9/E.png)

form_add.php

![App Screenshot](./lab7web/image/praktikum9/F.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/G.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/H.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/I.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/J.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/K.png)
form_edit.php

![App Screenshot](./lab7web/image/praktikum9/L.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/M.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/N.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/O.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/P.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/Q.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/R.png)

form_edit.php

![App Screenshot](./lab7web/image/praktikum9/S.png)

## PRAKTIKUM 10

Langkah-langkah Praktikum
Persiapan
Buka Kembali project sebelumnya, kemudian kita tambahkan Pustaka yang dibutuhkan
pada project tersebut.
Menambahkan Pustaka jQuery.
Kita akan menggunakan pustaka jQuery untuk mempermudah proses AJAX. Download
pustaka jQuery versi terbaru dari https://jquery.com dan ekstrak filenya.
Salin file jquery-3.6.0.min.js ke folder public/assets/js.
Membuat Model.
Pada modul sebelumnya sudah dibuat ArtikelModel, pada modul ini kita akan
memanfaatkan model tersebut agar dapat diakses melalui AJAX.
Membuat AJAX Controller


![App Screenshot](./lab7web/image/praktikum10/A.png)

Membuat View

![App Screenshot](./lab7web/image/praktikum10/B.png)
![App Screenshot](./lab7web/image/praktikum10/C.png)
![App Screenshot](./lab7web/image/praktikum10/D.png)
![App Screenshot](./lab7web/image/praktikum10/E.png)
![App Screenshot](./lab7web/image/praktikum10/F.png)
![App Screenshot](./lab7web/image/praktikum10/G.png)
![App Screenshot](./lab7web/image/praktikum10/H.png)

## PRAKTIKUM 11

Langkah-langkah Praktikum
1. Persiapan
* Pastikan MySQL Server sudah berjalan.
* Buka database `lab_ci4`.
* Pastikan tabel `artikel` dan `kategori` sudah ada dan terisi data.
* Pastikan library jQuery sudah terpasang atau dapat diakses melalui CDN.
2. Modifikasi Controller Artikel
Ubah method `admin_index()` di `Artikel.php` untuk mengembalikan data dalam format
JSON jika request adalah AJAX. (Sama seperti modul sebelumnya)

![App Screenshot](./lab7web/image/praktikum11/A.png)
![App Screenshot](./lab7web/image/praktikum11/B.png)
![App Screenshot](./lab7web/image/praktikum11/C.png)
![App Screenshot](./lab7web/image/praktikum11/D.png)
![App Screenshot](./lab7web/image/praktikum11/E.png)
![App Screenshot](./lab7web/image/praktikum11/F.png)
![App Screenshot](./lab7web/image/praktikum11/G.png)
![App Screenshot](./lab7web/image/praktikum11/H.png)

## PRAKTIKUM 12

Langkah-langkah Praktikum
Persiapan
Periapan awal adalah mengunduh aplikasi REST Client, ada banyak aplikasi yang dapat digunakan untuk
keperluan tersebut. Salah satunya adalah Postman. Postman – Merupakan aplikasi yang berfungsi
sebagai REST Client, digunakan untuk testing REST API. Unduh apliasi Postman dari tautan berikut:
https://www.postman.com/downloads/
Membuat Model.
Pada modul sebelumnya sudah dibuat ArtikelModel, pada modul ini kita akan memanfaatkan model
tersebut agar dapat diakses melalui API.
Membuat REST Controller
Pada tahap ini, kita akan membuat file REST Controller yang berisi fungsi untuk menampilkan,
menambah, mengubah dan menghapus data. Masuklah ke direktori app\Controllers dan buatlah file
baru bernama Post.php. Kemudian, salin kode di bawah ini ke dalam file tersebut:

![App Screenshot](./lab7web/image/praktikum12/A.png)

![App Screenshot](./lab7web/image/praktikum12/B.png)

![App Screenshot](./lab7web/image/praktikum12/C.png)

![App Screenshot](./lab7web/image/praktikum12/D.png)

![App Screenshot](./lab7web/image/praktikum12/E.png)

![App Screenshot](./lab7web/image/praktikum12/F.png)

![App Screenshot](./lab7web/image/praktikum12/G.png)

![App Screenshot](./lab7web/image/praktikum12/H.png)

![App Screenshot](./lab7web/image/praktikum12/I.png)

![App Screenshot](./lab7web/image/praktikum12/J.png)