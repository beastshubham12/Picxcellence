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

