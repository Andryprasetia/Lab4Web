# Pemograman Web
~~~
Nama  : Andry Prasetia perdana
NIM   : 311910284
Kelas : TI19C1
~~~
# 1.Membuat dokumen HTML
Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.
~~~
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
~~~
![Screenshot (67)](https://user-images.githubusercontent.com/81818989/116058741-55db0400-a6aa-11eb-8adf-b14616c7f581.png)
# 2. Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.
~~~
<section>
<div class="div1">Div 1</div>
<div class="div2">Div 2</div>
<div class="div3">Div 3</div>
</section>
~~~
![Screenshot (68)](https://user-images.githubusercontent.com/81818989/116058928-8884fc80-a6aa-11eb-91e0-d3c88f69df4e.png)
# 3. CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.
~~~
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
</style>
~~~
![Screenshot (69)](https://user-images.githubusercontent.com/81818989/116059041-a5b9cb00-a6aa-11eb-8e62-4030216d19cb.png)
# 4. Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk mengaturnya. Tambahkan element div lainnya seteleah div3 seperti berikut.
~~~
<section>
<div class="div1">Div 1</div>
<div class="div2">Div 2</div>
<div class="div3">Div 3</div>
<div class="div4">Div 4</div>
</section>
~~~
Kemudian atur property clear pada CSS, seperti berikut.
~~~
.div4 {
background-color: blue;
clear: left;
float: none;
}
~~~
![Screenshot (70)](https://user-images.githubusercontent.com/81818989/116059195-caae3e00-a6aa-11eb-982b-ab3cde217339.png)
# 5. Membuat Layout Sederhana
Kita akan membuat layout web sederhana,
Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css.
~~~
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
~~~
Kemudian buat kerangka layout dengan semantics element,
Kemudian tuliska source berikut
~~~
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
~~~
![Screenshot (71)](https://user-images.githubusercontent.com/81818989/116059492-195bd800-a6ab-11eb-83c0-4033fb4b7807.png)
Kemudian tambahkan kode CSS untuk membuat layoutnya.
~~~
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
color: #b5b5b5;
}
~~~
![Screenshot (72)](https://user-images.githubusercontent.com/81818989/116059592-32648900-a6ab-11eb-84e0-325ca051c142.png)
# 6. Membuat Navigasi
Kemudian selanjutnya mengatur navigasi.
~~~
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
~~~
![Screenshot (73)](https://user-images.githubusercontent.com/81818989/116059705-5031ee00-a6ab-11eb-80fb-133d42676fa4.png)
# 7. Membuat Hero Panel.
Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.
~~~
<section id="hero">
<h1>Hello World!</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
<a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
~~~
~~~
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
~~~
![Screenshot (75)](https://user-images.githubusercontent.com/81818989/116059821-75bef780-a6ab-11eb-943e-c108ce4e3091.png)
![Screenshot (76)](https://user-images.githubusercontent.com/81818989/116059851-81122300-a6ab-11eb-9274-dbe20a62c549.png)
# 8. Mengatur Layout Main dan Sidebar
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
~~~
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
~~~
![Screenshot (77)](https://user-images.githubusercontent.com/81818989/116059927-95eeb680-a6ab-11eb-90dc-ce426ed755e5.png)
# 9. Membuat Sidebar Widget
Kemudian selanjutnya menambahkan element lain dalam sidebar.
~~~
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
~~~
Kemudian tambahkan CSS.
~~~
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
~~~
![Screenshot (78)](https://user-images.githubusercontent.com/81818989/116060068-b6b70c00-a6ab-11eb-8b03-67f4df1abbda.png)
![Screenshot (80)](https://user-images.githubusercontent.com/81818989/116060097-bf0f4700-a6ab-11eb-85f5-16c63202908d.png)
# 10. Mengatur Footer
Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
~~~
/* footer */
footer {
clear:both;
background-color:#1d1d1d;
padding:20px;
color:#eee;
}
~~~
![Screenshot (81)](https://user-images.githubusercontent.com/81818989/116060220-df3f0600-a6ab-11eb-872f-e71674118e8b.png)
# 11. Menambahkan Elemen lainnya pada Main Content
~~~
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
~~~
kemudian tambahkan CSS
~~~
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
~~~
![Screenshot (82)](https://user-images.githubusercontent.com/81818989/116060331-fa117a80-a6ab-11eb-94b8-c5796691f4df.png)
![Screenshot (83)](https://user-images.githubusercontent.com/81818989/116060367-03024c00-a6ac-11eb-92a7-ff4fdb382bd8.png)
# 12. Menambahkan Content Artikel
Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.
~~~
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
~~~
Kemudian tambahkan CSS.
~~~
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
~~~
![Screenshot (84)](https://user-images.githubusercontent.com/81818989/116060643-3f35ac80-a6ac-11eb-9acf-16aa1f4aa6e3.png)
![Screenshot (85)](https://user-images.githubusercontent.com/81818989/116060705-4d83c880-a6ac-11eb-9fd6-9c387c8d57c8.png)
# Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll
![Screenshot (86)](https://user-images.githubusercontent.com/81818989/116060809-642a1f80-a6ac-11eb-83d5-a6a01382bc90.png)

2. Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll
![Screenshot (87)](https://user-images.githubusercontent.com/81818989/116060881-75732c00-a6ac-11eb-8142-5fa1463344d4.png)
