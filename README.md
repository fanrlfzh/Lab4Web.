#membuat Box Element
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
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div> 
</section>

#CSS Float Property
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
![Screenshot (247)](https://github.com/user-attachments/assets/c15ca268-7c55-4725-8e6b-505b57395bb6)

#Mengatur Clearfix Element
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div> 
 <div class="div4">Div 4</div> 
</section>
.div4 {
 background-color: blue;
 clear: left;
 float: none;
}
![Screenshot (248)](https://github.com/user-attachments/assets/5dbe1abd-f69f-437d-81ad-0c6b3b28012c)

#Membuat Layout Sederhana
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
![Screenshot (249)](https://github.com/user-attachments/assets/43bd39ed-d91d-4fb3-9528-5a42b06cc64d)

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
![Screenshot (250)](https://github.com/user-attachments/assets/7931ac07-60de-478f-92dd-357ac9c3ad70)

#Membuat Navigasi
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
![Screenshot (251)](https://github.com/user-attachments/assets/7810d419-7602-413b-87a9-2e3597e68c11)

#Membuat Hero Panel.
<section id="hero">
 <h1>Hello World!</h1>
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p>
 <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
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
![Screenshot (252)](https://github.com/user-attachments/assets/f7ab7689-0584-4644-94df-308a32015466)

#Mengatur Layout Main dan Sidebar
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

#Membuat Sidebar Widget
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
![Screenshot (253)](https://github.com/user-attachments/assets/1cccc339-15d0-494f-86a2-d2f0944e671b)

#Mengatur Footer
/* footer */
footer {
 clear:both;
 background-color:#1d1d1d;
 padding:20px;
 color:#eee;
}
![Screenshot (254)](https://github.com/user-attachments/assets/b72271cb-0b65-4681-abcf-edf4356bca28)

#Menambahkan Elemen lainnya pada Main Content
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
![Screenshot (255)](https://github.com/user-attachments/assets/f0141780-1663-4c25-96d8-81c33c8e1187)

#Menambahkan Content Artikel
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
![Screenshot (256)](https://github.com/user-attachments/assets/5509bf40-3f67-49ce-9140-252e5e48c85a)

#memvalidasi dokumen html
![Screenshot (259)](https://github.com/user-attachments/assets/70ab60e9-290a-44a2-b69e-0b3b2a536a36)

Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>About Me</h1>
        </header>

        <section class="about">
            <h2>Deskripsi</h2>
            <p>Saya adalah seorang profesional di bidang teknologi dengan pengalaman dalam pengembangan perangkat lunak dan manajemen proyek. Fokus saya adalah pada pengembangan aplikasi web dan mobile, serta optimasi sistem untuk efisiensi yang lebih baik.</p>
        </section>

        <section class="portfolio">
            <h2>Portfolio</h2>
            <div class="portfolio-grid">
                <div class="portfolio-item">
                    <img src="portfolio1.jpg" alt="Project 1">
                    <p>Project 1: Aplikasi e-commerce.</p>
                </div>
                <div class="portfolio-item">
                    <img src="portfolio2.jpg" alt="Project 2">
                    <p>Project 2: Platform pembelajaran online.</p>
                </div>
                <div class="portfolio-item">
                    <img src="portfolio3.jpg" alt="Project 3">
                    <p>Project 3: Aplikasi manajemen tugas.</p>
                </div>
            </div>
        </section>

        <section class="contact">
            <h2>Kontak</h2>
            <p>Email: contoh.email@gmail.com</p>
            <p>Telepon: +62 812 3456 7890</p>
        </section>

        <footer>
            <p>&copy; 2024 About Me. All Rights Reserved.</p>
        </footer>
    </div>
</body>
</html>
/* Import Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700&display=swap');

/* Reset CSS */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Body Styling */
body {
    font-family: 'Open Sans', sans-serif;
    color: #333;
    background-color: #f4f4f4;
    line-height: 1.6;
}

/* Kontainer Utama */
#container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

/* Header */
header {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: #fff;
}

header h1 {
    font-size: 2.5em;
    margin-bottom: 0.5em;
}

/* Section About */
.about {
    padding: 20px 0;
}

.about h2 {
    font-size: 2em;
    color: #333;
}

.about p {
    font-size: 1.1em;
    margin-top: 10px;
    line-height: 1.8;
}

/* Section Portfolio */
.portfolio {
    padding: 20px 0;
}

.portfolio h2 {
    font-size: 2em;
    color: #333;
    margin-bottom: 20px;
}

.portfolio-grid {
    display: flex;
    justify-content: space-between;
    gap: 20px;
    flex-wrap: wrap;
}

.portfolio-item {
    background-color: #f9f9f9;
    padding: 15px;
    width: 30%;
    text-align: center;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.portfolio-item img {
    max-width: 100%;
    height: auto;
    margin-bottom: 10px;
}

.portfolio-item p {
    font-size: 1em;
    color: #555;
}

/* Section Contact */
.contact {
    padding: 20px 0;
    text-align: center;
}

.contact h2 {
    font-size: 2em;
    color: #333;
}

.contact p {
    font-size: 1.1em;
    margin: 10px 0;
    color: #555;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: #fff;
    margin-top: 20px;
}

/* Layout Responsif */
@media (max-width: 768px) {
    .portfolio-grid {
        flex-direction: column;
        gap: 10px;
    }

    .portfolio-item {
        width: 100%;
    }
}
![Screenshot (257)](https://github.com/user-attachments/assets/898e88bd-60cd-48ae-9270-d0b913a68a91)

2. Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Contact Us</h1>
        </header>

        <section class="contact-form">
            <h2>Get in Touch</h2>
            <form action="#" method="POST">
                <label for="name">Name</label>
                <input type="text" id="name" name="name" placeholder="Your Name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" placeholder="Your Email" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" rows="6" placeholder="Your Message" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </section>

        <footer>
            <p>&copy; 2024 Contact Us. All Rights Reserved.</p>
        </footer>
    </div>
</body>
</html>
/* Import Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700&display=swap');

/* Reset CSS */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Body Styling */
body {
    font-family: 'Open Sans', sans-serif;
    color: #333;
    background-color: #f4f4f4;
    line-height: 1.6;
}

/* Kontainer Utama */
#container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

/* Header */
header {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: #fff;
}

header h1 {
    font-size: 2.5em;
    margin-bottom: 0.5em;
}

/* Section Contact Form */
.contact-form {
    padding: 20px 0;
}

.contact-form h2 {
    font-size: 2em;
    color: #333;
    text-align: center;
    margin-bottom: 20px;
}

.contact-form form {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
}

.contact-form label {
    margin: 10px 0 5px;
    font-weight: 600;
}

.contact-form input,
.contact-form textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 1em;
    margin-bottom: 15px;
    background-color: #f9f9f9;
}

.contact-form input:focus,
.contact-form textarea:focus {
    outline: none;
    border-color: #666;
}

.contact-form button {
    padding: 15px;
    background-color: #333;
    color: #fff;
    font-size: 1.2em;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.contact-form button:hover {
    background-color: #555;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: #fff;
    margin-top: 20px;
}

/* Layout Responsif */
@media (max-width: 768px) {
    .contact-form form {
        width: 100%;
    }
}
![Screenshot (258)](https://github.com/user-attachments/assets/843e619e-35ba-49fb-b3f3-1faca51511b9)















