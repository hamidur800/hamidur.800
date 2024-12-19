<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Protfolio_Mahfuz</title>
    <link rel="stylesheet" href="styel.css">
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
    <link rel="icon" href="img/1.png">
  <style> *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins', sans-serif;
    text-decoration: none;
}

body {
   

}

a{
    color: #fff;
}

.navbar{
    position: fixed;
    left: 0;
    top: 0;
    width: 100%;
    padding: 25px 9%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
    visibility: hidden;
    opacity: 0;
    animation: show-content 1.5s linear forwards;
    animation-delay: 1.2s;
}

@keyframes show-content {
    100% {
        visibility: visible;
        opacity: 1;
    }
}
.navbar .logo {
    font-size: 30px;
    font-weight: 700;
    
}
.navbar ul {
    display: flex;
    

}
.navbar ul li {
    list-style: none;
    margin-left: 35px;
}
.navbar ul li a {
    
    font-size: 20px;
    font-weight: 500;
    transition: .5s;
}
.navbar ul li:hover a,
.navbar ul li.active a{
    color: #7cf03d;
}
.home {
    display: flex;
    gap: 50px;
    align-items: center;
    height: 100vh;
    padding: 60px 9% 0;
    color: #fff;
    visibility: hidden;
    opacity: 0;
    animation: show-content 1.5s linear forwards;
    animation-delay: 1.6s;
}
.home-info h1 {
    font-size: 50px;

}
.home-info h2 {
    display: inline-block;
    font-size: 32px;
    margin-top: -10px;
    
}
/*content stert*/
.home-info h2 span {
    position: relative;
    display: inline-block;
    color: transparent;
    -webkit-text-stroke: .7px #7cf03d;
     animation: display-text 16s linear infinite; 
    animation-delay: calc(-4s * var(--1));
}
@keyframes display-text {
    25%,100% {
        display: none;
    }
}

.home-info h2 span::before {
    content: attr(data-text);
    position: absolute;
    width: 0;
    border-right: 2px solid #7cf03d;
    color: #7cf03d;
    white-space: nowrap;
    overflow: hidden;
    animation: fill-text 4s linear infinite;
}
@keyframes fill-text {
    10%,
    100% {
        width: 0;
    }
    70%,
    90% {
        width: 100%;
    }
}

/*content end*/

.home-info p {
    font-size: 16px;
    margin: 10px 0 25px;
}
.home-info .btn-sci {
    display: flex;
    align-items: center;
}
.btn {
    display: inline-block;
    padding: 10px 30px;
    background: #7cf03d;
    border: 2px solid #7cf03d;
    border-radius: 40px;
    box-shadow: 0 0 10px #7cf03d;
    font-size: 16px;
    color: #1f242d;
    font-weight: 600;
    transition: .5s;
}
.btn:hover {
    background: transparent;
    color: #7cf03d;
    box-shadow: none;
}
.home-info .btn-sci .sci  {
    margin-left: 20px;
}
.home-info .btn-sci .sci a {
    display: inline-flex;
    padding: 8px;
    border: 2px solid #7cf03d;
    border-radius: 50%;
    font-size: 20px;
    color: #7cf03d;
    margin: 0 8px;
    transition: .5s;
}
.home-info .btn-sci .sci a:hover {
    background: #7cf03d;
    color: #1f242d;
    box-shadow: 0 0 10px;
}
/*navbar*/

.home-img .img-box {
    position: relative;
    width: 32vw;
    height: 32vw;
    border-radius: 50%;
    padding: 5px;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;

}
.home-img .img-box::before,
.home-img .img-box::after {
    content: '';
    position: absolute;
    width: 500px;
    height: 500px;
    background: conic-gradient(transparent,transparent,transparent,#7cf03d);
    transform: rotate(0deg);
    animation: rotate-border 10s linear infinite;
}

.home-img .img-box::after {
    animation-delay: -5s;
}

@keyframes rotate-border {
    100% {
        transform: rotate(360deg);
    }
}
.home-img .img-box .img-item {
    position: relative;
    width: 100%;
    height: 100%;
    background: #1f242d;
    border-radius: 50%;
    border: .1px solid #1f242d;
    display: flex;
    justify-content: center;
    z-index: 1;
    overflow: hidden;
}
.home-img .img-box .img-item img {
    position: absolute;
    display: block;
    width: 85%;
    object-fit: cover;
    mix-blend-mode: lighten;

}

/*animition section stert*/
.bars-animation {
     position: absolute;
     width: 100%;
     height: 100%;
     display: flex;
     z-index: -1;

}
.bars-animation .bar {
    width: 100%;
    height: 100%;
    background: #1f242d;
    transform: translateY(-100%);
    animation: show-bars .5s ease-in-out forwards;
    animation-delay: calc(.1s * var(--1));
}
@keyframes show-bars {
    100% {
        transform: translateY(0%);
    }
}

/*animition section end*/</style>
</head>
<body>
    <!--navbar section start-->
 <nav class="navbar">
   <a href="#"class="logo">MAHFUZ.</a>
   <ul>
    <li class="active"><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Portfolio</a></li>
    <li><a href="#">Service</a></li>
    <li><a href="#">Contact</a></li>
   </ul>

 </nav>
    <!--navbar section end-->
    <!--animition section stert-->

      <div class="bars-animation">
        <div class="bar" style="--1:6;"></div>
        <div class="bar" style="--1:5;"></div>
        <div class="bar" style="--1:4;"></div>
        <div class="bar" style="--1:3;"></div>
        <div class="bar" style="--1:2;"></div>
        <div class="bar" style="--1:1;"></div>
      </div>

    <!--animition section end-->
     
    <!--home section stert-->
    <section class="home">
        <div class="home-info">
            <h1>Mahfuzur Rahman</h1>
            <h2>I'm a
                <span style="--1:4;" data-text="Frontend Web Developer"> Frontend Web Developer</span>
                <span style="--1:3;" data-text="Student">Student</span>
                <span style="--1:2;" data-text="Speed Learner">Speed Learner</span>
                <span style="--1:1;" data-text="Web Designer">Web Designer</span>
            </h2>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illum nesciunt quia officiis sunt  iusto, dicta ipsa sequi tempore!</p>
            <div class="btn-sci">
              <a href="#" class="btn">Download CV</a>
              <div class="sci">
                 <a href="https://github.com/mahfuz3026" target="_blank"><i class='bx bxl-github'></i></a>
                 <a href="#"><i class='bx bxl-linkedin-square'></i></a>
                 <a href="#"><i class='bx bxl-twitter'></i></a>
                 <a href="#"><i class='bx bxl-youtube'></i></a>
              </div>
            </div>
        </div>
        <!--img stert-->
        <div class="home-img">
            <div class="img-box">
                <div class="img-item">
                    <img src="img/prop.png" alt="">
                </div>
            </div>
        </div>
        <!--img stert-->
    </section>
    <!--home section end-->
</body>
</html>
