@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    scroll-behavior: smooth;
    font-family: 'Poppins',sans-serif;
}
:root{
    --bg-color:#081b29;
    --second-bg-color:#112e42;
    --text-color:#ededed;
    --main-color:#00abf0;
}
html{
    font-size: 62.5%;
    overflow-x: hidden;
}
body{
    background: var(--bg-color);
    color: var(--text-color);
}
.header{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 2rem 9%;
    background: transparent;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100%;
    transition: .3s;
}
.header.sticky{
    background: var(--bg-color);
}
.logo{
    position: relative;
    font-size: 2.5rem;
    color: var(--text-color);
    font-weight: 600;
}
.navbar{
    position: relative;
}
.navbar a{
    font-size: 1.7rem;
    color: var(--text-color);
    font-weight: 500;
    margin-left: 3.5rem;
    transition: .3s;
}
.navbar a:hover,
.navbar a.active{
    color: var(--main-color);
}
#menu-icon{
    position: relative;
    font-size: 3.6rem;
    color: var(--text-color);
    cursor: pointer;
    display: none;
}
section{
    min-height: 100vh;
    padding: 10rem 9% 2rem;
}
.home{
    display: flex;
    align-items: center;
    padding: 0 9%;
    background: url(../image/home.jpg);
    background-size: cover;
    background-position: center;
}
.home-content{
    max-width: 60rem;
    z-index: 99;
}
.home-content h1{
    position: relative;
    display: inline-block;
    font-size: 5.2rem;
    font-weight: 700;
    line-height: 1.3;
}
.home-content h1 span{
    color: var(--text-color);
}
.home-content .text-animate{
    position: relative;
    width: 50.8rem;
}
.home-content .text-animate h3{
    font-size: 3.2rem;
    font-weight: 700;
    color: transparent;
    -webkit-text-stroke: .7px var(--main-color);
   background-image: linear-gradient(var(--main-color),var(--main-color));
    background-repeat: no-repeat;
    background-position: -52rem 0;
    /*animation: homeBgText 6s linear infinite;
    animation-delay: 2s;*/
}
.home-content .text-animate h3::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    border-right: 2px solid var(--main-color);
    z-index: -1;
    animation: homeCursorText 6s linear infinite;
    animation-delay: 2s;
}
.home-content p{
    position: relative;
    font-size: 1.6rem;
    margin: 2rem 0 4rem;
}
.btn-box{
    position: relative;
    display: flex;
    justify-content: space-between;
    width: 34.5rem;
    height: 5rem;
}
.btn-box .btn{
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 15rem;
    height: 100%;
    background: var(--main-color);
    border: .2rem solid var(--main-color);
    border-radius: .8rem;
    font-size: 1.8rem;
    font-weight: 600;
    letter-spacing: .1rem;
    color: var(--bg-color);  
    z-index: 1;
    overflow: hidden;
    transition: .5s;
}
.btn-box .btn:hover{
    color: var(--main-color);
}
.btn-box .btn:nth-child(2){
    background: transparent;
    color: var(--main-color);
}
.btn-box .btn:nth-child(2):hover{
    color : var(--main-color);
}
.btn-box .btn:nth-child(2)::before{
    background: var(--main-color);
}
.btn-box .btn::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background:var(--bg-color);
    z-index: -1;
    transition: .5s;
}
.btn-box .btn:hover:before{
    width: 100%;
}
.home-sci{
    position: absolute;
    bottom: 4rem;
    width: 170px;
    display: flex;
    justify-content: space-between;
}
.home-sci a {
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 40px;
    height: 40px;
    background: transparent;
    border: .2rem solid var(--main-color);
    border-radius: 50%;
    font-size: 20px;
    color: var(--main-color);
    z-index: 1;
    overflow: hidden;
    transition: .5s;
}
.home-sci a:hover{
    color: var(--bg-color);
}
.home-sci a::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width:  0;
    height: 100%;
    background:var(--main-color);
    z-index: -1;
    transition: .5s;
}
home-sci a:hover::before{
    width: 100%;
}
.home-imgHover{
    position: absolute;
    top: 7.7rem;
    right: 0;
    width: 45%;
    height: 90%;
    background: transparent;
    transition: 3s; 
}
.home-imgHover:hover{
    background: var(--bg-color);
    opacity: .2;
}

.about{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 2rem;
    background: var(--second-bg-color);
    padding-bottom: 6rem;
}
.heading{
    position: relative;
    font-size: 5rem;
    margin-bottom: 3rem;
    text-align: center;
}
span{
    color: var(--main-color);
}
.about-img{
    position: relative;
    width: 25rem;
    height: 25rem;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.about-img img{
    width: 82%;
    border-radius: 10%;
    border: .2rem solid var(--main-color);
}
.about-img .circle-spin{
    position:absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%) rotate(0);
    width: 90%;
    height: 130%;
    border-radius: 10%;
    border-top: .2rem solid red;
    border-bottom: .2rem solid red;
    border-left: .2rem solid var(--main-color);
    border-right: .2rem solid var(--main-color);

}
.about-content{
    text-align: center;
    
}
.about-content h3{
    position: relative;
    display: inline-block;
    font-size: 2.6rem;
    margin-top: 30px;
}
.about-content p{
    position: relative;
    font-size: 1.6rem;
    margin: 2rem 0 3rem;
}
.btn-box.btns{
    display: inline-block;
    width: 40rem;
    height: 55px;
    font-size: 1.6rem;
}
.btn-box.btns a::before{
background: var(--second-bg-color);
}

.education{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: auto;
    padding-bottom: 5rem;
    

}
.education .education-row{
    display: flex;
    flex-wrap: wrap;
    gap: 5rem;

}
.education-row .education-column{
    flex: 1 1 40rem;

}
.education-column .title{
    position: relative;
    display: inline-block;
    font-size: 3rem;
    margin: 0 0 1.5rem 2rem;
}
.education-column .education-box{
    position: relative;
    border-left: .2rem solid var(--main-color);

}
.education-box .education-content{
    position: relative;
    padding-left: 2rem;
}
.education-box .education-content::before{
    content: '';
    position: absolute;
    top: 0;
    left: -1.1rem;
    width: 2rem;
    height: 2rem;
    background: var(--main-color);
    border-radius: 50%;
}
.education-content .content{
    position: relative;
    padding: 1.5rem;
    border: .2rem solid var(--main-color);
    border-radius: .6rem;
    margin-bottom: 2rem;
    overflow: hidden;
}
.education-content .content::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background:var(--second-bg-color);
    z-index: -1;
    transition: .5s;
}
.education-content .content:hover::before{
    width: 100%;
}
.education-content .content .year{
    font-size: 1.8rem;
    color: var(--main-color);
    padding-bottom: .5rem;

}
.education-content .content .year i{
    padding-right: .5rem;
}
.education-content .content h3{
    font-size: 2.5rem;
}
.education-content .content p{
    font-size: 2rem;
    padding-top: .5rem;
}

.skills{
    min-height: auto;
    padding: 7rem;
    background: var(--second-bg-color);
}
.skills h2{
    display: inline-block;
    left: 50%;
    transform: translateX(-50%) ;
}
.skills .skills-row{
    display: flex;
    flex-wrap: wrap;
    gap: 5rem;
}
.skills-row .skills-column{
    flex: 1 1 40rem;
}
.skills-column .title{
    position: relative;
    display: inline-block;
    font-size: 2.5rem;
    margin: 0 0 1.5rem;
}
.skills-column .skills-box{
    position: relative;
}
.skills-box .skills-content{
    position: relative;
    border: .2rem solid var(--main-color);
    border-radius: .6rem;
    padding: .5rem 1.5rem;
    z-index: 1;
    overflow: hidden;
}
.skills-box .skills-content::before{
    content: '';
    position:absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background:var(--bg-color);
    z-index: -1;
    transition: .5s;
}
.skills-box .skills-content:hover::before{
    width: 100%;
}
.skills-content .progress{
    padding: 1rem 0;
}
.skills-content .progress h3{
    font-size: 1.7rem;
    display: flex;justify-content: space-between;
}
.skills-content .progress h3 span{
    color: var(--text-color);
}
.skills-content .progress .bar{
    height: 2.5rem;
    border-radius: .6rem;
    border: .2rem solid var(--main-color);
    padding: .5rem;
    margin: 1rem 0;
}
.skills-content .progress .bar span{
    display: block;
    height: 100%;
    border-radius: .3rem;
    background: var(--main-color);
}
.skills-column:nth-child(1) .skills-content .progress:nth-child(1) .bar span{
    width: 80%;
}
.skills-column:nth-child(1) .skills-content .progress:nth-child(2) .bar span{
    width: 70%;
}
.skills-column:nth-child(1) .skills-content .progress:nth-child(3) .bar span{
    width: 85%;
}
.skills-column:nth-child(1) .skills-content .progress:nth-child(4) .bar span{
    width: 90%;
}
.skills-column:nth-child(2) .skills-content .progress:nth-child(1) .bar span{
    width: 80%;
}
.skills-column:nth-child(2) .skills-content .progress:nth-child(2) .bar span{
    width: 70%;
}
.skills-column:nth-child(2) .skills-content .progress:nth-child(3) .bar span{
    width: 85%;
}
.skills-column:nth-child(2) .skills-content .progress:nth-child(4) .bar span{
    width: 90%;
}

.contact{
    min-height: auto;
    padding-bottom: 7rem;
}
.contact h2{
    display: inline-block;
    left: 50%;
    transform: translateX(-50%);
}
.contact form{
    max-width: 70rem;
    margin: 0 auto;
    text-align: center;
}
.contact form .input-box{
    position: relative;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}
.contact form .input-box .input-field{
    position: relative;
    width: 49%;
    margin: .8rem 0;
}
.contact form .input-box .input-field input,
.contact form .textarea-field textarea{
    width: 100%;
    height: 100%;
    padding: 1.5rem;
    font-size: 1.6rem;
    color: var(--text-color);
    background: transparent;
    border-radius: .6rem;
    border: .2rem solid var(--main-color);
}
.contact form .input-box .input-field input::placeholder,
.contact form .textarea-field textarea::placeholder{
    color: var(--text-color);
}
.contact  form .focus{
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: var(--second-bg-color);
    border-radius: .6rem;
    z-index: -1;
    transition: .5s;
}
.contact form .input-box .input-field input:focus~.focus ,
.contact form .input-box .input-field input:valid~.focus ,
.contact form .textarea-field textarea:focus~.focus ,
.contact form .textarea-field textarea:valid~.focus {
    width: 100%;
}
.contat form .textarea-field{
    position: relative;
    margin: .8rem 0 2.7rem;
    display: flex;
}
.contat form .textarea-field textarea{
    resize: none;
}
.contact form .btn-box.btns .btn{
    cursor: pointer;
}

.footer{
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    padding: 2rem 9%;
    background: var(--second-bg-color);
}
.footer-text,
.footer-icons{
    position: relative;
}

.footer-text a{
    font-size: 2rem;
    color: var(--text-color);
}
.footer-icons a{
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    padding: .8rem;
    background-color: var(--main-color);
    border: .2rem solid var(--main-color);
    border-radius: .6rem;
    z-index: 1;
    overflow: hidden;
}
.footer-icons a::before{
    content: '';
    position:absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background:var(--bg-color);
    z-index: -1;
    transition: .5s;

}
.footer-icons a:hover::before{
    width: 100%;
}
.footer-icons a i{
    font-size: 2.4rem;
    color: var(--bg-color);
    transition: .5s;

}
.footer-icons a:hover i{
    color:var(--main-color) ;
}

/*ANIMATION RELOAD AND SCROLL
animate{
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background: yellowgreen;
    z-index: 98;
} */
.animate.home-img{
    width: 90%;
}
.logo .animate,
.navbar .animate,
#menu-icon .animate,
.home.show-animate .animate{
    animation: showRight 1s ease forwards;
    animation-delay: calc(.3s*var(--i));
}
.animate.scroll{
    transition: 1s ease;
    transition-delay:calc(.3s/var(--i)) ;
    animation: none;
}
.education .education-box .animate.scroll{
    width: 105%;
}
.about.show-animate .animate.scroll,
.education.show-animate .animate.scroll,
.skills.show-animate .animate.scroll,
.footer.show-animate .animate.scroll{
    transition-delay:calc(.3s*var(--i)) ;
    width: 0;    
}

/*BREAK POINTS*/
@media(max-width:1200px){
    html{
        font-size: 55%;
    }
}

@media(max-width:991px){
    .header{
        padding: 2rem 4%;
    }
    section{
        padding: 10rem 4% 2rem;
    }

    .home{
        padding: 0 4%;
    }

    .footer{
        padding: 2rem 4%;
    }
}

@media(max-width:768px){
    .header{
        background: var(--bg-color);
    }
    #menu-icon{
        display: block;
    }
    .navbar{
        position: absolute;
        top: 100%;
        left: -100%;
        width: 100%;
        padding: 1rem 4%;
        background: var(--main-color); 
        box-shadow: 0 .5rem 1rem rgba(0, 0,0, .2);
        z-index: 1;
        transition: .25s ease;
        transition-delay: .25s;
    }
    .navbar.active{
        left: 0;
        transition-delay: 0s;
    }
    .navbar .active-nav{
        position: absolute;
        top: 0;
        left: -100%;
        width: 100%;
        height: 100%;
        background: var(--bg-color);
        border-top: .1rem solid rgba(0, 0,0, .2);
        z-index: -1;
        transition: .25s ease;
        transition-delay: 0s;
    }
    .navbar.active .active-nav{
        left: 0;
        transition-delay: .25s;
        
    }
    .navbar a{
        display: block;
        font-size: 2rem;
        margin: 3rem 0;
        transform: translateX(-20rem);
        transition: .25s ease;
        transition-delay: 0s;
    }
    .navbar.active a{
        transform: translateX(0);
        transition-delay: .25x;
    }
    .home-imgHover{
        pointer-events: none;
        background: var(--bg-color);
        opacity: .6;
    }
}

@media(max-width:520px){
    html{
        font-size: 50%;
    }
    .home-content h1{
        display: flex;
        flex-direction: column;
    }
    .home-sci{
        width: 160px;
    }
    .home-sci a{
        width: 38px;
        height: 38px;
    }
}
@media(max-width:462px){
    .home-content h1{
        font-size: 5.2rem;
    }
    .education{
        padding: 10rem 4% 5rem 5%;
    }
    .contact form .input-box .input-field{
        width: 100%;
    }
    .footer{
        flex-direction: column-reverse;
    }
    .footer p{
        margin-top: 2rem;
        text-align: center;
    }
}
@media(max-width:371px){
    .home{
        justify-content: center;
    }
    .home-content{
        display: flex;
        align-items: center;
        flex-direction: column;
        text-align: center;
    }
    .home-content h1{
        font-size: 5rem;
    }
}


/*KEYFRAMES ANIMATION*/
@keyframes homeBgText{
    0%,10%,100%{
        background-position: -33rem 0;
    }
    65%,
    85%{
        background-position: 0 0;
    }
}

@keyframes homeCursorText{
    0%,
    10%,
    100%{
        width: 0;
    }
    65%,
    78%,
    85%{
        width: 51%;
        opacity: 1;
    }
    75%,
    81%{
        opacity: 0;
    }
}

@keyframes showRight{
    100%{
        width: 0;
    }
}
CSS
//toggle icon navbar
let menuIcon=document.querySelector('#menu-icon');
let navbar=document.querySelector('.navbar');

menuIcon.onclick = () => {
    menuIcon.classList.toggle('bx-x');
    navbar.classList.toggle('active');
}

//scroll sections
let sections = document.querySelectorAll('section');
let navLinks = document.querySelectorAll('header nav a');


window.onscroll = () => {
    sections.forEach(sec => {
        let top=window.scrollY;
        let offset=sec.offsetTop - 100;
        let height=sec.offsetHeight;
        let id=sec.getAttribute('id');


        if(top >= offset && top < offset + height){
            //active navbar links
            navLinks.forEach(links => {
                links.classList.remove('active');
                document.querySelector('header nav a[href*=' +id+ ']').classList.add('active');
            });
            //active section for animation on scroll
            sec.classList.add('show-animate');
        }
        //if want to use animation that repats on scroll this
        else{
            sec.classList.remove('show-animate');
        }
    });
    //sticky header
    let header=document.querySelector('header');

    header.classList.toggle('sticky',window.scrollY > 100);

    //remove toggle icon and navbar when click navbar links (scroll)

    menuIcon.classList.remove('bx-x');
    navbar.classList.remove('active');

    //animation footer on scroll.
    let footer = document.querySelector('footer');

    footer.classList.toggle('show-animate', this.innerHeight + this.scrollY >= document.scrollingElement.scrollHeight);

}
JAVASCRIPT
HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VARUNKUMAR S</title>
    <link rel="stylesheet" href="./css/style.css">
    <!--box icons-->
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
</head>
<body>
    <!--HEADER DESIGN-->
    <header class="header">
        <a href="#" class="logo"><span style="color: #00abf0; font-size: 5rem;">V</span>arun.<span class="animate" style="--i:1;"></span></a>
        <div class="bx bx-menu" id="menu-icon"><span class="animate" style="--i:2;"></span></div>
        <nav class="navbar">
            <a href="#home" class="active">Home</a>
            <a href="#about">About</a>
            <a href="#education">Education</a>
            <a href="#skills">Skills</a>
           <!-- <a href="#contact">Contact</a>-->

            <span class="active-nav"></span>
            <span class="animate" style="--i:2;"></span>
        </nav>
    </header>
    <!--HOME SECTION DESIGN-->
    <section class="home show-animate" id="home">
        <div class="home-content">
            <h1>Hi, I'm <span>VARUNKUMAR S</span><span class="animate" style="--i:2;"></span></h1>
            <div class="text-animate">
                <h3>Java Developer</h3>
                <span class="animate" style="--i:3;"></span>
            </div>
            <p>A passionate Java Developer with recent degree in Bachelor of Engineering 
                from Government college of Engineering, Dharmapuri. I recently graducated with a degree in Computer Science, where I gained
                hands-on experience with Java programming. I have a strong foundation in Java, Object-Oriented Programming (OOP). I am also familiar with Web Technologies 
                like HTML, CSS, and databases such as MySQL.
                <span class="animate" style="--i:4;"></span></p>
            <div class="btn-box">
                <a href="mailto:varunvijay016@gmail.com" class="btn">Mail Me</a>
                <a href="tel:+918248229870" class="btn">Let's Talk  <i class='bx bx-phone-call'></i></a>
                <span class="animate" style="--i:5;"></span>
            </div>

        </div>
        <div class="home-sci">
            <a href="https://wa.me/918248229870?text=Hello, Varunkumar S"><i class='bx bxl-whatsapp' ></i></a>
            <a href="#"><i class='bx bxl-github'></i></i></a>
            <a href="https://www.linkedin.com/in/varunkumar-s-java-developer"><i class='bx bxl-linkedin' ></i></a>
            <span class="animate" style="--i:6;"></span>
        </div>
        <div class="home-imgHover">
            
            <span class="animate home-img" style="--i:7;"></span>
        </div>
    </section>
    <!--ABOUT SECTION DESIGN-->
    <section class="about" id="about">
        <h2 class="heading">About <span>Me</span><span class="animate scroll" style="--i:1;"></span></h2>
        <div class="about-img">
            <img src="./image/about.png" alt="">
            <span class="circle-spin"></span>
            <span class="animate scroll" style="--i:2;"></span>
        </div>
        <div class="about-content">
            <h3>Java Developer!<span class="animate scroll" style="--i:3;"></span></h3>
            <p>Hello, I' m  <b style="font-size: 25px;">VARUNKUMAR S</b> ,  a passionate Java Developer with recent degree in Bachelor of Engineering 
                from Government college of Engineering, Dharmapuri. I recently graducated with a degree in Computer Science, where I gained
                hands-on experience with Java programming. I have a strong foundation in Java, Object-Oriented Programming (OOP). I am also familiar with Web Technologies 
                like HTML, CSS, and databases such as MySQL. " I' m eager to continue expanding my knowledge of Java and explore areas such as Spring framework and web development.
                My goal is to innovative software solutions and grow as a developer". "Feel free to browse through my portfolio to see my projects, and don't 
                hesitate to reach out if you'd like to discuss potential opportunities!"

                <span class="animate scroll" style="--i:4;"></span></p>
        
            <div class="btn-box btns">
                <a href="./image/Varunkumar.pdf" class="btn" download="Varunkumar S-Resume" >DOWNLOAD<i class='bx bx-down-arrow-alt' style="font-size: 30px;"></i></a>
                <span class="animate scroll" style="--i:5;"></span>
            </div>
        </div>
    </section>
    <!--EDUCATION SECTION DESIGN-->
    <section class="education" id="education">
        <h2 class="heading">My <span>Journey</span><span class="animate scroll" style="--i:1;"></span></h2>
        <div class="education-row">
            <div class="education-column">
                <h3 class="title">Education<span class="animate scroll" style="--i:2;"></span></h3>

                <div class="education-box">
                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar' ></i>2020-2024</div>
                            <h3>Bachelor Degree-Anna University</h3>
                            <h1 style="color: #f5f7fa; font-size: 2.5rem;">B.E - CSE</h1>
                            <p>Government college of Engineering, Dharmapuri </p>
                            <p style="color: #f5f7fa; font-size: 2rem;">CGPA: <b>7.0</b></p>

                        </div>
                    </div>
                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar' ></i>2019-2020</div>
                            <h3>HSC-State Board</h3>
                            <p>Kanakadasa matric hr.sec.school,<br>Bargur </p>
                            <p style="color: #f5f7fa; font-size: 2rem;">Percentage: <b>78%</b></p>

                        </div>
                    </div>
                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar' ></i>2017-2018</div>
                            <h3>SSLC-State Board</h3>
                            <p>Selva matric hr.sec.school,<br>Bargur</p>
                            <p style="color: #f5f7fa; font-size: 2rem;">Percentage: <b>86%</b></p>

                        </div>
                    </div>
                    <span class="animate scroll" style="--i:3;"></span>
                </div>
            </div>

            
            <div class="education-column">
                <h3 class="title">Experience<span class="animate scroll" style="--i:5;"></span></h3>

                <div class="education-box">
                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar' ></i>2022-2023</div>
                            <h3>Project-1</h3>
                            <p style="color: #f5f7fa; font-size: 2rem;">Title: <b>Kidney Tumour Segmentation</b></p>
                            <p>Kidney tumour segmentation using nnUnet on CT-SCAN and developed a website using Flask.</p>

                        </div>
                    </div>
                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar' ></i>2023-2024</div>
                            <h3>Project-2</h3>
                            <p style="color: #f5f7fa; font-size: 2rem;">Title: <b>Portfolio Website</b></p>
                            <p style="color: #f5f7fa; font-size: 1.8rem;">A Portfolio Website is a digital space that showcases your work,skills, and experiences. 
                                It can be used to share your work with potential employers, collaborators, or the press. </p>


                        </div>
                    </div>
                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar' ></i>2022-2023</div>
                            <h3>Internship</h3>
                            <p style="color: #f5f7fa; font-size: 2rem;">Title: <b>Web Development</b></p>
                            <p>I attended an internship in Web Development domain provided by NSIC at EKKADUTHANGAL.</p>

                        </div>
                    </div>
                    <span class="animate scroll" style="--i:6;"></span>
                </div>
            </div>
        </div>
    </section>
    <!--SKILLS SECTION DESIGN-->
    <section class="skills" id="skills">
        <h2 class="heading">My <span>Skills</span><span class="animate scroll" style="--i:1;"></span></h2>

        <div class="skills-row">
            <div class="skills-column">
                <h3 class="title">Coding Skills<span class="animate scroll" style="--i:2;"></span></h3>

                <div class="skills-box">
                    <div class="skills-content">
                        <div class="progress">
                            <h3>HTML <span>80%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                        <div class="progress">
                            <h3>CSS <span>70%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                        <div class="progress">
                            <h3>JAVA <span>85%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                        <div class="progress">
                            <h3>SQL <span>90%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                    </div>
                    <span class="animate scroll" style="--i:3;"></span>
                </div>
            </div>
            <div class="skills-column">
                <h3 class="title">Professional Skills<span class="animate scroll" style="--i:5;"></span></h3>

                <div class="skills-box">
                    <div class="skills-content">
                        <div class="progress">
                            <h3>web design <span>80%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                        <div class="progress">
                            <h3>web development <span>70%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                        <div class="progress">
                            <h3>JAVA development<span>85%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                        <div class="progress">
                            <h3>SQL development <span>90%</span></h3>
                            <div class="bar"><span></span></div>
                        </div>
                    </div>
                    <span class="animate scroll" style="--i:6;"></span>
                </div>
            </div>
        </div>
    </section>
    <!--CONTACT SECTION DESIGN
    <section class="contact" id="contact">
        <h2 class="heading">Contact <span>Me!</span><span class="animate scroll" style="--i:1;"></span></h2>

        <form action="#">
            <div class="input-box">
                <div class="input-field">
                    <input type="text" placeholder="Full Name" required>
                    <span class="focus"></span>
                </div>
                <div class="input-field">
                    <input type="text" placeholder="Email Address" required>
                    <span class="focus"></span>
                </div>
                <span class="animate scroll" style="--i:3;"></span>
            </div>
            <div class="input-box">
                <div class="input-field">
                    <input type="number" placeholder="Mobile Number" required>
                    <span class="focus"></span>
                </div>
                <div class="input-field">
                    <input type="text" placeholder="Email Subject" required>
                    <span class="focus"></span>
                </div>
                <span class="animate scroll" style="--i:5;"></span>
            </div>

            <div class="textarea-field">
                  
                 <textarea name="" id="" cols="30" rows="10" placeholder="Your Message" required></textarea>
                 <span class="focus"></span>
                 <span class="animate scroll" style="--i:7;"></span>
            </div>

            <div class="btn-box btns">
                <button type="submit" class="btn">Submit</button>
                <span class="animate scroll" style="--i:9;"></span>
            </div>
        </form>

    </section>-->
    <!--FOOTER SECTION DESIGN-->
    <footer class="footer">
        <div class="footer-text">
          <a href="https://www.linkedin.com/in/varunkumar-s-java-developer"><p><b style="font-size: 2.5rem;">Linkedin:</b> "https://www.linkedin.com/in/varunkumar-s-java-developer"</p></a>  
            <span class="animate scroll" style="--i:1;"></span>
        </div>
        <div class="footer-icons">
             <a href="#"><i class='bx bx-up-arrow-alt' ></i></a>
             <span class="animate scroll" style="--i:3;"></span>
        </div>
    </footer>



    <script src="./js/script.js"></script>
</body>
</html>
