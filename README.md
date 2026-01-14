<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Wastu Nirman Pvt. Ltd.</title>

<style>
/* RESET */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins', Arial, Helvetica, sans-serif;
}

/* BODY */
body{
    background:linear-gradient(135deg,#fdfbfb,#ebedee);
    color:#333;
    scroll-behavior: smooth;
    overflow-x: hidden;
}

/* HEADER */
header{
    background:linear-gradient(90deg,#ff8a00,#e52e71);
    color:#fff;
    padding:40px 20px;
    text-align:center;
    position:relative;
    overflow:hidden;
}
header::after{
    content:"";
    position:absolute;
    width:300px;
    height:300px;
    background:rgba(255,255,255,0.1);
    border-radius:50%;
    top:-50px;
    right:-50px;
    animation: float 8s infinite ease-in-out alternate;
}
@keyframes float{
    0%{transform: translateY(0) rotate(0deg);}
    100%{transform: translateY(20px) rotate(360deg);}
}
header h1{
    font-size:48px;
    letter-spacing:2px;
    margin-bottom:10px;
    text-shadow:2px 2px 8px rgba(0,0,0,0.2);
}
header p{
    font-size:18px;
    font-weight:500;
}

/* NAVBAR */
nav{
    background:#1a1a1a;
    display:flex;
    justify-content:center;
    position:sticky;
    top:0;
    z-index:1000;
    box-shadow:0 5px 15px rgba(0,0,0,0.3);
}
nav a{
    color:#fff;
    text-decoration:none;
    padding:15px 25px;
    font-weight:500;
    transition:0.3s;
    border-radius:5px;
    margin:5px;
}
nav a:hover{
    background:#ff8a00;
    color:#fff;
    transform: scale(1.1);
}

/* HERO */
.hero{
    background:url('https://i.supaimg.com/686c6869-df74-42b1-9c4b-1b9020d92472.jpg') center/cover no-repeat;
    height:500px;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    color:#fff;
    position:relative;
}
.hero::before{
    content:"";
    position:absolute;
    width:100%;
    height:100%;
    background:rgba(0,0,0,0.5);
}
.hero h2{
    position:relative;
    font-size:48px;
    padding:25px 40px;
    border-radius:15px;
    background:rgba(255,255,255,0.1);
    backdrop-filter: blur(5px);
    box-shadow:0 10px 25px rgba(0,0,0,0.3);
    animation: fadeIn 2s ease-in-out forwards;
}
@keyframes fadeIn{
    from{opacity:0; transform: translateY(20px);}
    to{opacity:1; transform: translateY(0);}
}

/* SECTION */
.section{
    padding:80px 20px;
    max-width:1200px;
    margin:auto;
}
.section h2{
    text-align:center;
    margin-bottom:60px;
    font-size:36px;
    color:#e52e71;
    position:relative;
}
.section h2::after{
    content:"";
    width:80px;
    height:3px;
    background:#ff8a00;
    display:block;
    margin:10px auto 0;
    border-radius:2px;
}

/* SERVICES */
.services{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:30px;
}
.service-box{
    background:#fff;
    padding:35px 25px;
    text-align:center;
    border-radius:15px;
    box-shadow:0 15px 30px rgba(0,0,0,0.1);
    transition:0.5s;
    position:relative;
    overflow:hidden;
}
.service-box::before{
    content:"";
    position:absolute;
    width:120%;
    height:120%;
    background:linear-gradient(45deg,#ff8a00,#e52e71);
    top:100%;
    left:-10%;
    transition:0.5s;
    transform:rotate(25deg);
    z-index:0;
}
.service-box:hover::before{
    top:-10%;
}
.service-box h3{
    margin-bottom:15px;
    color:#e52e71;
    position:relative;
    z-index:1;
}
.service-box p{
    color:#555;
    position:relative;
    z-index:1;
}

/* PORTFOLIO */
.portfolio{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}
.portfolio img{
    width:100%;
    border-radius:15px;
    box-shadow:0 15px 35px rgba(0,0,0,0.2);
    transition:0.5s;
}
.portfolio img:hover{
    box-shadow:0 25px 50px rgba(0,0,0,0.3);
    transform: none; /* zoom/rotate effect हटाइयो */
}

/* CONTACT */
.contact{
    background:linear-gradient(135deg,#ff8a00,#e52e71);
    padding:40px;
    border-radius:20px;
    color:#fff;
    text-align:center;
    box-shadow:0 15px 35px rgba(0,0,0,0.2);
    transition:0.5s;
}
.contact p{
    font-size:18px;
    margin:15px 0;
}
.contact:hover{
    transform: scale(1.02);
}

/* FOOTER */
footer{
    background:#111;
    color:#fff;
    text-align:center;
    padding:25px;
    margin-top:40px;
    font-size:14px;
    letter-spacing:1px;
}

/* RESPONSIVE */
@media(max-width:600px){
    header h1{font-size:32px;}
    .hero h2{font-size:28px;}
    nav a{padding:12px 15px;}
    .section{padding:50px 15px;}
}
</style>
</head>

<body>

<header id="home">
    <h1>WASTU NIRMAN Pvt. Ltd.</h1>
    <p>House & Building Construction Company</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#portfolio">Portfolio</a>
    <a href="#contact">Contact</a>
</nav>

<section class="hero">
    <h2>We Will Make Your Dream House 
From Planing Designing To Construction</h2>
</section>

<section id="services" class="section">
    <h2>Our Services</h2>
    <div class="services">
        <div class="service-box">
            <h3>New Construction</h3>
            <p>Residential & commercial construction from foundation to finish.</p>
        </div>
        <div class="service-box">
            <h3>2D & 3D Blueprint</h3>
            <p>Modern architectural design and planning solutions.</p>
        </div>
        <div class="service-box">
            <h3>Renovation</h3>
            <p>Upgrade and remodel your existing building beautifully.</p>
        </div>
        <div class="service-box">
            <h3>Roofing</h3>
            <p>Strong and weather-resistant roofing solutions.</p>
        </div>
    </div>
</section>

<section id="portfolio" class="section">
    <h2>Our Portfolio</h2>
    <div class="portfolio">
        <img src="https://i.supaimg.com/5450a869-22af-4dc3-9d94-0cb3eb491aab.jpg">
        <img src="https://i.supaimg.com/897c7339-8f00-40f0-91fd-0e5fee3a673d.jpg">
        <img src="https://i.supaimg.com/99d530e3-76ea-44a7-9845-741d70eb8547.jpg">
        <img src="https://i.supaimg.com/82745204-e9a4-4d85-bf57-84a54fbc344d.jpg">
    </div>
</section>

<section id="contact" class="section">
    <h2>Contact Us</h2>
    <div class="contact">
        <p><strong>Email:</strong> wastunirman@gmail.com</p>
        <p><strong>Phone:</strong> 9808827962, 9823135299</p>
        <p><strong>Location:</strong> Nepal</p>
    </div>
</section>

<footer>
    <p>&copy; 2025 Wastu Nirman Pvt. Ltd. All Rights Reserved.</p>
</footer>

</body>
</html>
