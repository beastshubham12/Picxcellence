# Picxcellence
My first repository

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">
    <link rel="stylesheet" type="text/css" href="sty.css">
    <link rel="stylesheet" type="text/css" href="./css/font-awesome.min.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.1.1/css/fontawesome.min.css" integrity="sha384-zIaWifL2YFF1qaDiAo0JFgsmasocJ/rqu7LKYH8CoBEXqGbb9eO+Xi3s6fQhgFWM" crossorigin="anonymous">
</head>

<body>
    <header>
        <nav>
            <div class="logo">
                Pic<span>X</span>cellence
            </div>
            <div class="menu">
                <a href="home">Home</a>
                <a href="about">About</a>
                <a href="gallery">Gallery</a>
                <a href="contact">Contact</a>
            </div>

            <div class="icon">
                <i class="fas fa-search" aria-hidden="true"></i>
                <a href="#">Login</a>
            </div>
        </nav>
        <section class="h-text">
            <i class="fas fa-camera"></i>
            <h1>Capturing moments that captivate your heart</h1>
            <input type="text" name="" placeholder="Search here....">
            <button><i class="fas fa-search"></i></button>
        </section>
    </header>
    <section class="filter-gallery">
        <div class="portfolio-menu">
            <ul>
                <li class="active" data-filter="*">All</li>
                <li data-filter=".nature">Nature</li>
                <li data-filter=".wedding">Mountains</li>
                <li data-filter=".fashion">Fashion</li>
            </ul>
        </div>
        <div class="portfolio-item">
            <div class="item nature">
                <img src="p1.jpg" width="100" height="100">
            </div>
            <div class="item fashion">
                <img src="p2.jpg" width="100" height="100">
            </div>
            <div class="item wedding">
                <img src="p3.jpg" width="100" height="100">
            </div>
            <div class="item nature">
                <img src="p4.jpg" width="100" height="100">
            </div>
            <div class="item fashion">
                <img src="p5.jpg" width="100" height="100">
            </div>
            <div class="item wedding">
                <img src="p6.jpg" width="100" height="100">
            </div>
            <div class="item nature">
                <img src="p7.jpg" width="100" height="100">
            </div>
            <div class="item fashion">
                <img src="p8.jpg" width="100" height="100">
            </div>
            <div class="item wedding">
                <img src="p9.jpg" width="100" height="100">
            </div>

        </div>
    </section>
    <br>
    <section class="member">
        <div class="area">
            <ul class="circles">
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
            </ul>

            <div class="member-info">
                <h1>Our<span> Information</span></h1>
                <p>What our member says</p>
            </div>
            <div class="member-card">
                <img src="ingj.jpg" alt="myself" width="100">
                <p>
                    Nature photography is a wide range of photography taken outdoors and devoted to displaying natural elements such as landscapes, wildlife, plants, and close-ups of natural scenes and textures.
                </p>
                <h1>*Shubham Bhattacharjee</h1>
                <h2>
                    <a href="www.instagram.com"><i class="fab fa-youtube"></i></a>
                    <a href="www.youtube.com"><i class="fab fa-instagram"></i></a>
                    <a href="www.gmail.com"><i class="fas fa-envelope"></i></a>
                </h2>
            </div>
        </div>

        <div class="m-images">
            <img src="s1.jpg">
            <img src="s2.jpg">
            <img src="s3.jpg">
            <img src="s4.jpg">
            <img src="s5.jpg">
            <img src="s6.jpg">
        </div>

    </section>
    <footer>
        <div class="newsletter">
            <div>
                <h2>Subscribe to our Youtube Channel</h2>
                <p>We're a team of non-cynics who truly care for our work.</p>
            </div>
            <div>
                <label>
            <input type="text" name="" placeholder="Enter your email">
            <button>Subscribe</button>
        </label>
            </div>
        </div>

    </footer>

    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous">
    </script>
    <script src="https://unpkg.com/isotope-layout@3/dist/isotope.pkgd.min.js">
    </script>
    <script type="text/javascript">
        $('.portfolio-item').isotope({
            // options
            itemSelector: '.item',
            layoutMode: 'fitRows'
        });
        $('.portfolio-menu ul li').click(function() {
            $('.portfolio-menu ul li').removeClass('active');
            $(this).addClass('active');

            var selector = $(this).attr('data-filter');
            $('.portfolio-item').isotope({
                filter: selector
            });
            return false;
        });
    </script>



</body>

</html>

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

.body {
    scroll-behavior: smooth;
    overflow-x: hidden;
}

header {
    width: 100%;
    height: 95vh;
    background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url(ibnh.jpg);
    background-size: cover;
    background-attachment: fixed;
}

nav {
    width: 100%;
    height: 80px;
    background: white;
    color: black;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0px 80px;
    top: 0;
}

.logo {
    font-family: serif;
    font-size: 50px;
}

.logo span {
    color: rgb(235, 23, 16);
}

.menu a {
    color: black;
    padding: 10px 20px;
    font-family: sans-serif;
    font-size: 20px;
    text-decoration: none;
}

.menu a :first-child {
    color: red;
}

.menu a:hover {
    color: chartreuse;
}

.icon i {
    font-variation-settings: '\f002';
    font-size: 20px;
}

.icon i:hover {
    color: burlywood;
}

.icon a {
    text-decoration: none;
    background: #e74c3c;
    color: white;
    padding: 10px 20px;
    margin: left 30px;
    border-radius: 5px;
}

.h-text {
    color: white;
    max-width: 700px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
}

.h-text i {
    font-variation-settings: '\f030';
    align-items: center;
    font-size: 50px;
}

.h-text i :hover {
    color: aquamarine;
}

.h-text h1 {
    font-family: sans-serif;
    font-size: 3em;
    line-height: 1.5em;
}

.h-text input {
    width: 60%;
    padding: 20px;
    border: none;
    outline: none;
    font-size: 20px;
    border-radius: 8px;
}

.h-text button {
    width: 30%;
    padding: 20px;
    background: #e74c3c;
    color: white;
    border: none;
    outline: none;
    border-radius: 8px;
    font-size: 20px;
    margin-top: 30px;
}

.h-text button i {
    font-variation-settings: '\f002';
    font-size: 25px;
}

.filter-gallery {
    padding: 100px;
}

.portfolio-menu {
    text-align: center;
    margin-bottom: 20px;
}

.portfolio-menu ul li {
    list-style: none;
    display: inline-block;
    margin: 20px 0px;
    font-size: 20px;
    font-weight: bold;
    font-family: sans-serif;
    padding: 10px 20px;
    cursor: pointer;
    transition: 0.5s ease;
    text-align: center;
}

.portfolio-menu ul li:hover {
    color: white;
    background: #e74c3c;
    border-radius: 8px;
}

li.active {
    color: white;
    background: #e74c3c;
    border-radius: 8px;
}

.portfolio-item {
    width: 100%;
}

.portfolio-item .item {
    width: 360px;
    height: 360px;
    float: left;
    margin-bottom: 20px;
    margin-right: 20px;
}

.portfolio-item .item img {
    width: 100%;
    height: 100%;
    border-radius: 8px;
}

.member {
    width: 100%;
    padding: 20px 100px;
    font-family: sans-serif;
}

.member-info {
    text-align: center;
}

.member-info h1 {
    font-size: 2.5em;
}

.member-info h1 span {
    color: #e74c3c;
}

.member-card {
    text-align: center;
    padding-top: 50px;
    width: 50%;
    margin: auto;
}

.member-card p {
    margin: 20px 0px;
    line-height: 2em;
}

.member-card a img:hover {
    color: darkorange;
}

.member-card img {
    border-radius: 8px;
}

.m-images {
    width: 100%;
    display: flex;
    margin: 20px 0px;
    overflow: hidden;
}

.m-images img {
    width: 200px;
    height: 200px;
    cursor: pointer;
    transition: 0.4s ease-in-out;
}

.m-images img:hover {
    transform: scale(1.5);
}

footer {
    width: 100%;
    height: 30vh;
    background: #111111;
    padding: 50px 100px;
}

.newsletter {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px;
    border: 1px solid rgba(225, 225, 225, 0.2);
}

.newsletter>div {
    flex-basis: 50%;
    color: white;
}

.ntext {
    text-align: right;
}

.newsletter h2 {
    font-size: 2em;
    font-family: sans-serif;
}

.newsletter p {
    font-size: 20px;
    margin-top: 10px;
}

.newsletter label {
    position: relative;
}

.newsletter input {
    padding: 20px;
    width: 70%;
    border-radius: 8px;
    border: none;
    outline: none;
    font-family: sans-serif;
}

.newsletter button {
    position: absolute;
    right: 0;
    padding: 20px;
    width: 30%;
    background: #e74c3c;
    color: white;
    border: none;
    border-radius: 0 8px 8px 0;
}

@import url('https://fonts.googleapis.com/css?family=Exo:400,700');
* {
    margin: 0px;
    padding: 0px;
}

.area {
    background: #4e54c8;
    background: -webkit-linear-gradient(to left, #8f94fb, #4e54c8);
    width: 100%;
    height: 60vh;
}

.circles {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    overflow: hidden;
}

.circles li {
    position: absolute;
    display: block;
    list-style: none;
    width: 20px;
    height: 20px;
    background: rgba(255, 255, 255, 0.2);
    animation: animate 25s linear infinite;
    bottom: -150px;
}

.circles li:nth-child(1) {
    left: 25%;
    width: 80px;
    height: 80px;
    animation-delay: 0s;
}

.circles li:nth-child(2) {
    left: 10%;
    width: 20px;
    height: 20px;
    animation-delay: 2s;
    animation-duration: 12s;
}

.circles li:nth-child(3) {
    left: 70%;
    width: 20px;
    height: 20px;
    animation-delay: 4s;
}

.circles li:nth-child(4) {
    left: 40%;
    width: 60px;
    height: 60px;
    animation-delay: 0s;
    animation-duration: 18s;
}

.circles li:nth-child(5) {
    left: 65%;
    width: 20px;
    height: 20px;
    animation-delay: 0s;
}

.circles li:nth-child(6) {
    left: 75%;
    width: 110px;
    height: 110px;
    animation-delay: 3s;
}

.circles li:nth-child(7) {
    left: 35%;
    width: 150px;
    height: 150px;
    animation-delay: 7s;
}

.circles li:nth-child(8) {
    left: 50%;
    width: 25px;
    height: 25px;
    animation-delay: 15s;
    animation-duration: 45s;
}

.circles li:nth-child(9) {
    left: 20%;
    width: 15px;
    height: 15px;
    animation-delay: 2s;
    animation-duration: 35s;
}

.circles li:nth-child(10) {
    left: 85%;
    width: 150px;
    height: 150px;
    animation-delay: 0s;
    animation-duration: 11s;
}

@keyframes animate {
    0% {
        transform: translateY(0) rotate(0deg);
        opacity: 1;
        border-radius: 0;
    }
    100% {
        transform: translateY(-1000px) rotate(720deg);
        opacity: 0;
        border-radius: 50%;
    }
}
