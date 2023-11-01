# Lab6web

# Membuat Layout sederhana
## Kerangka Layout
![layout](https://github.com/DimasF3009/Lab4web/assets/115356128/5e579e29-ae42-4d52-9e57-b08eb28ae20c)
## Membuat folder html
```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

</body>
</html>
```
## Import Bundle dari Boostrap
### Import Bundle Css
```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
```
### Import Bundle JS
```
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
```
## Membuat Navigasi
Membuat navigasi menggunakan html
```
<header><h1>Berita Masa Kini</h1></header>
    <nav>
      <ul>
        <a href="web.html" class="active">Home</a>
        <a href="#main">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Contact</a>
      </ul>
    </nav>
```
Kemudian tambahkan css kedalam html
```
*{
    padding: 0;
    margin: 0;
}
/* layout CSS */
#main {
    float: left;
    width: 640px;
    padding: 19px;
}

/* BODY */
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#6b6969;
}

/* container */
#container {
    width: 980px;
    height: 2000px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

/* Header */
header{
    padding: 10px;
    background-color: #ddd8d8;
}
header h1 {
    margin: 20px 10px;
    color: #181616;
}

/* WRAPPER */
#wrapper{
    margin: 0px;
}

/* Navigasi */
nav{
    display: block;
    background-color: rgb(207, 5, 5);
    padding: 5px;
}
ul a{
    color: white;
    display: inline-block;
    padding: 5px;
    margin: 5px;
    text-decoration: none;
}
```
### Hasil
<img width="960" alt="hasil3" src="https://github.com/DimasF3009/Lab4web/assets/115356128/8b04255a-9720-4b46-8b49-bad62e1ac15f">

## Membuat Slide show 
Membuat slideshow dengan boostrap
```
      <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="/gambar/indonesia1.png" class="d-block w-100" alt="indonesia1">
            <div class="carousel-caption d-none d-md-block">
      
            </div>
          </div>
          <div class="carousel-item">
            <img src="/gambar/indonesia2.jpg" class="d-block w-100" alt="indonesia2">
            <div class="carousel-caption d-none d-md-block">
              
            </div>
          </div>
          <div class="carousel-item">
            <img src="/gambar/indonesia3.jpg" class="d-block w-100" alt="indonesia3">
            <div class="carousel-caption d-none d-md-block">
            
            </div>
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
```
## Hasil
![pict1](https://github.com/DimasF3009/Lab6web/assets/115356128/cb6bbbf3-d0b5-4907-b83a-0071c6d0ecf1)


## Membuat Sidebar
Membuat sidebar dengan html
```
<section id="wrapper">
      <aside id="sidebar">
          <div class="side-bar">
            <h3 class="title">Other News</h3>
            <ul>
              <li><a href="#">Sport News</a></li>
              <li><a href="#">Political News</a></li>
              <li><a href="#">Economic News</a></li>
              <li><a href="#">Environmental News</a></li>
              <li><a href="#">Domestic News</a></li>
            </ul>
          </div>
          <div class="side-bar">
            <h3 class="title">Widget Text</h3>
            <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt 
              arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer 
              pharetra est nunc, nec pretium nunc pretium ac.</p>
          </div>
      </aside>
</section>
```
Kemudian tambahkan css kedalam html
```
#sidebar{
    float: left;
    width: 260px;
    padding: 20px;
}
.side-bar .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}    
.side-bar {
    border:1px solid #eee;
    margin-bottom:20px;
}
.side-bar ul{
    list-style: none; 
}
.side-bar ul li{
   border-bottom:1px solid #eee;
}
.side-bar a{
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}
.side-bar li:hover a {
    background-color:#eee;
}
.side-bar p {
    padding:15px;
    line-height:25px;
}
```
### Hasil
<img width="268" alt="hasil7" src="https://github.com/DimasF3009/Lab4web/assets/115356128/c69a3912-6093-49fa-a6bd-91c090ba1c72">

## Membuat Main content
Membuat main content dengan html
```
<section id="wrapper">
    <section id="main">
        <article class="artikel">
          <p>
            KEMENKO PMK --  Indonesia akan mengalami usia emas pada tahun 2045. Pada saat itu, Indonesia genap berusia 100 tahun alias satu abad. Di masa itu, ditargetkan Indonesia sudah menjadi negara maju dan telah sejajar dengan negara adidaya. 
          </p><br>
          <p>
            Momentum bersejarah tersebut memang masih sekitar saperempat abad lagi. Namun untuk mewujudkannya butuh persiapan yang matang sejak jauh-jauh hari. Sumber daya manusia Indonesia harus unggul, berkualitas, dan memiliki karakter. 
          </p><br>
          <p>
            Menteri Koordinator Bidang Pembangunan Manusia dan Kebudayaan (Menko PMK) Muhadjir Effendy mengatakan, generasi yang akan mewujudkan Indonesia Emas adalah generasi muda, khususnya yang saat ini tengah menempuh pendidikan di perguruan tinggi.
          </p><br>
          <p>
            Dia menerangkan, para mahasiswa/mahasiswi dan lulusan universitas jenjang sarjana saat ini berada di kisaran usia 20 tahun. Menurutnya, pada masa Indonesia berusia 100 tahun yaitu 2045, usia mereka masih sekitar 40 tahun ke atas, yang merupakan usia puncak karir bagi profesional.
          </p><br>
          <p>
            "Artinya, Indonesia Emas itu adalah milik saudara semua, bukan milik saya. Bukan milik mereka yang saat ini usianya sudah di atas 50 tahun," ujar Muhadjir saat menyampaikan sambutan pada Wisuda Ke-105 Periode III Universitas Muhammadiyah Malang (UMM), di UMM Dome Malang, pada Kamis (6/10/2022).
          </p>
        </article>
    </section>
</section>
```
Kemudian tambahkan css kedalam html
```
.artikel{
   margin-left: 10px;
   padding: 30px;
}
.artikel p{
    font-size: 100%;
    justify-content: space-between;
}
```
### Hasi
<img width="833" alt="hasil8" src="https://github.com/DimasF3009/Lab4web/assets/115356128/abeab6ff-8bb5-454e-b63e-75b2fe6675aa">

## Membuat Artikel Lainnya
Membuat artikel lainnya dengan card content
```
            <article class="entry">
              <div class="card mb-3" style="max-width: 540px;">
                <div class="row g-0">
                  <div class="col-md-4">
                    <img src="/gambar/prabowo.jpg" class="img-fluid rounded-start" alt="prabowo" style="margin-top: 80px; margin-left: 10px;">
                  </div>
                  <div class="col-md-8">
                    <div class="card-body">
                      <h5 class="card-title">Prabowo Yakin Menang Pada Pemilu 2024 Ini</h5>
                      <p class="card-text" align = "justify"> Prabowo sudah dua kali maju jadi capres dan belum berhasil. Tapi kali ini dengan dukungan bersama dan keputusan yang tepat yang beliau ambil nanti saat pendaftaran calon presiden dan calon wakil presiden pada Oktober mendatang, insya Allah sekali ini Prabowo akan memenangkan pertarungan 
                        <a href="#">pilpres.</a></p>
                      <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                    </div>
                  </div>
                </div>
              </div>
            </article>
        
          <hr class="divider" />
    
            <article class="entry">
              <div class="card mb-3" style="max-width: 540px;">
                <div class="row g-0">
                  <div class="col-md-4">
                    <img src="/gambar/Icecold.jpeg" class="img-fluid rounded-start" alt="iceCold" style="margin-top: 50px;  margin-left: 10px;">
                  </div>
                  <div class="col-md-8">
                    <div class="card-body">
                      <h5 class="card-title">Ice Cold Documentary Film</h5>
                      <p class="card-text" align = "justify">Dokumenter ini mengulas berbagai pertanyaan tak terjawab seputar persidangan Jessica Wongso bertahun-tahun setelah kematian sahabatnya, Mirna Salihin.
                        Dengan menyaksikan dokumenter ini, mari bersama-sama memahami kasus ini <a href="#">lebih kompleks lagi.</a></p>
                      <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                    </div>
                  </div>
                </div>
              </div>
            </article>
```
### Hasil
![pict2](https://github.com/DimasF3009/Lab6web/assets/115356128/8b69f0e6-511e-40ef-86e4-e834097205fc)

## Membuat Footer
Membuat footer dengan html
```
    <footer>
      <div class="kontak">
        <h2><a href="kontak.html" style="text-decoration: none;">Contact</a></h2>
        <p>&#128383; 0812-9318-9221</p>
        <p><a href="kontak.html" style="text-decoration: none;">&#128386; dimasf.30@mhs.pelitabangsa.ac.id</a></p>
      </div>
      <div class="lisensi">
        <p>&copy; 2023 - Dimas Firmansyah</p>
      </div>
    </footer>
```
Kemudian tambahkan css kedalam html
```
footer{
    background-color: aqua;
    padding: 20px;
    margin: 10px;
    margin-bottom: 10px;
    border-radius: 10px;
}
.lisensi{
    float: right;
}
```
### Hasil
<img width="687" alt="hasil10" src="https://github.com/DimasF3009/Lab4web/assets/115356128/71afb517-cc9a-489c-a5ba-3f8a86ef5386">

### Tambahkan Layout untuk menu About
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About</title>
</head>
<style>
*{
    padding: 0px;
    margin: 0px;
}
body{
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#6b6969;
}
#container {
    width: 600px;
    height: 600px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
#wrapper{
  margin: 0px;
}
.gambar img{
  width: 100px;
  height: 100px;
  border-radius: 50%;
  padding: 10px;
  margin: 0px auto;
  display: block;
}
.desc{
  box-shadow: 0 0 1em #cccccc;
  border-radius: 10px;
  width: 500px;
  margin: 0px auto;
  display: block;
}
.desc p{
  padding: 5px;
}
.button{
  padding: 10px;
}
.button button{
  margin: 0px auto;
  display: block;
}
button a{
  text-decoration: none;
  margin: 0px auto;
  display: block;
  padding: 10px;
}
</style>
<body>
  <div id="container">
    <section class="about">
      <h1 align="center">About Me</h1>
      <hr>
    </section>

    <section id="wrapper">
      <div class="gambar">
        <img src="gambar/saya.png" alt="me">
      </div>
      <h1 align="center">Dimas Firmansyah</h1><br>
      <div class="desc">
        <p>
          Saya, Dimas Firmansyah, merupakan salah satu mahasiswa Universitas Pelita Bangsa.
        </p>
        <p>
          Saat ini, saya sedang menempuh jenjang sarjana di bidang teknik informatika, dan kami sedang mempelajari cara membuat tata letak website.
        </p>
        <p>
          Tata letak website adalah komponen yang sangat penting dalam proses pembuatan website, terutama untuk pengembangan desain dan pengalaman pengguna.
        </p>
        <p>
          Selain itu, tata letak website juga berfungsi untuk mempermudah para pengembang web dalam proses pembuatan website secara keseluruhan
        </p>

      </div>
    </section>

    <div class="button">
      <button><a href="home.html">Back to Content</a></button>
    </div>

  </div>
</body>
</html>
```
### Hasil
<img width="445" alt="hasil11" src="https://github.com/DimasF3009/Lab4web/assets/115356128/fb7a13a0-cbf9-49a0-b07f-66e5797317ce">

### Tambahkan layout untuk menu Contact
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form</title>
</head>
<style>
body{
    font-size:100%;
    font-family:'Open Sans', sans-serif;
}
.form{
    border: 2px solid #000;
    padding: 20px; 
    display: flex;
    flex-direction: column;
    max-width: 300px;
    margin: 0 auto;
    border-radius: 10px;
    background-color: aquamarine;
}
.title{
    border: 2px solid black;
    text-align: center;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    padding: 10px;
    box-shadow: 5px 10px black;
}
.title h1{
    font-size: 100%;
}
.button{
    column-gap: 10px;
    display: flex;
    margin: 0 auto;
}
</style>
<body>
   <div class="main">
        <form action="proses.php" method="post" class="form">
            <div class="title">
                <h1><b>Contact Me</b></h1>
            </div>
            <p>
                <label for="name">Nama:</label><br>
                <input type="text" id="name" name="name" placeholder="Masukkan Nama Anda">
            </p>
            <p>
                <label for="email">Email:</label><br>
                <input type="text" name="email" id="email" placeholder="Masukkan Email Anda">
            </p>
            <p>
                <label for="order">Pesan:</label><br>
                <textarea name="pesan" id="pesan" cols="30" rows="10" placeholder="Masukan Pesan Anda Disini"></textarea>
            </p>
            <div class="button">
                <p align = "center">
                    <button>
                        <a href="home.html" style="text-decoration: none;">Batal</a>
                    </button>
                <p align = "center">
                    <input type="submit" value="Kirim">
                </p>
            </div>
        </form>
   </div>
</body>
</html>
```
### hasil
<img width="278" alt="hasil12" src="https://github.com/DimasF3009/Lab4web/assets/115356128/a9bc71c8-b9a6-4738-904e-fe71f7a8b83f">





















