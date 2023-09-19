# PORTFOLIO_VKJ
This is a  portfolio website created using html ,css and javascript.

//HTML CODE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VARSHA _developer portfolio</title>
    <link rel="stylesheet" href="style1.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Labrada&family=Roboto:ital@1&display=swap" rel="stylesheet">
    <style>
        *{
            margin:0;
            padding:0;
        }
        body{
        background-color:rgb(0,0,33);
        color:white;
        font-family: 'Poppins', sans-serif;
        }
        nav{
            display: flex;
            justify-content: space-around;
            align-items:center;
            height: 70px;
            background-color: rgb(42, 42, 214);
        }
        nav ul{
            display: flex;
            justify-content: center;
        }
        nav ul li{
            list-style:none;
            margin:0 23px;
        }

        nav ul li a{
            text-decoration: none;
            color:white;
        }
        nav ul li :hover{
            color:rgb(209, 46, 204);
            font: size 1.04rem;
        }
        main hr
        {
            border:0;
            background: #9c97f1;
            height:1.2px;
            margin:40px 84px;

        }
        .left{
            font-size:1.5rem;
        }
        .firstSection{
            display: flex;
            justify-content: space-around;
            align-items:center;
            margin: 140px 0;


            
        }

        .firstSection > div{ 
            width:30%;
        }
        .leftSection{
            font-size: 3rem;
            margin:70px 0;

        }
        .rightSection img{
            
            width: 80%;
            margin: 50px 0;
        

        }
        .purple{
            color:rgb(225, 31, 250);
        }
        .text-gray
        {
            color:gray;
        }

        #element {
            color:rgb("170,107,228");

        }
        .secondSection
        {
            max-width:80vw;
            margin:auto;
            height:80vh;

        }

        .secondSection h1{
            font-size:1.9rem;
        }

        .secondSection .box {
            background: white;
            width:80vw;
            height: 2px;
            margin:56px 0;
            display: flex;
        }
        .secondSection .vertical{
            height:93px;
            width:1px;
            background-color: white;
            margin:0 100px;
        }
        .image-top{
            width: 23px;
            position:relative;
            top: -32px;
            left: -9px;
        }

        .vertical-title{
            position:relative;
            top:75px;
            width:150px;

        }
        .vertical-desc{
            position:relative;
            top:86px;
            color:gray;
            width:150px;
            font-size:9px;

        }


    </style>
</head>
<body>
    <header>
        <nav>
            <div class="left">Varsha's portfolio</div>
            <div class="right">
                <ul id="sidemenu">
                    <li><a href="#home">Home</a></li>                    
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#contact">Contact Me</a></li>
                    <i class="fa-sharp fa-solid fa-xmark" onclick="closemenu()"></i>
                </ul>
                <i class="fa-solid fa-bars" onclick="openmenu()"></i>
            </div>
        </nav>
    </header>
    <main>
        <section class="firstSection">
            <div class="leftSection">
                Hi, My name is <span class="purple">Varsha kumari</span> 
                <div>and I am a passionate</div>
               
                <span id="element"></span>
            </div>
            <div class="rightSection">
<img src="bg.png" alt="">
            </div>
        
    </main>
    <script src="https://unpkg.com/typed.js@2.0.16/dist/typed.umd.js"></script>

    <script>
        var typed = new Typed('#element', {
          strings: ['Web Developer','Graphic Designer','Web Designer','Web content writter!'],
          typeSpeed: 50,
        });
      </script>

<div id="about">
    <div class="container">
        <div class="row">
            <div class="about-col-1">
                <img src="img2.jpg" alt="error" height="200">
            </div>
            <div class="about-col-2">
                <h1 class="subtitle">About Me</h1>
                <p>I am ambitious and driven.I am passionate about my work and I know how to get the job done.Also, I would also like to mention that I am a very hardworking
                    person and whenever I do any kind of work ,I do it with
                    perfection. I am someone who likes to take up
                    challenges because challenges drives a person
                    towards perfection. And I always tries to learn new
                    things because what I feel is that no one knows
                    everything, everyone has to learn day-by-day to
                    enhance their knowledge.And I am someone who
                    always things twice or even thrice before making any
                    kind of decision.</p>

                <div class="tab-titles">
                    <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                    <p class="tab-links" onclick="opentab('achievements')">Achievements</p>
                    <p class="tab-links" onclick="opentab('education')">Education</p>
                </div>
                <div class="tab-contents active-tab" id="skills">
                    <ul>
                        
                        <li><span>WEB-DEVELOPMENT</span><br>Web app Development.</li>
                        <li><span>JAVA</span><br>Core Java </li>
                        <li><span>DSA</span><br>Data structures and Algorithms</li>
                    </ul>
                </div>

                <div class="tab-contents" id="achievements">
                    <ul>
                        <li><span>2022</span><br>Selected for finale in SMART ODISHA HACKTHON.</li>
                        <li><span>2023</span><br> Selected for finale in GDSE WOW HACKTHON</li>
                        <li><span>2022</span><br>Member of INSTITUTE INNOVATION COUNCIL</li>
                        
                    </ul>
                </div>
                <div class="tab-contents" id="education">
                    <ul>
                        <li><span>DAV PUBLIC SCHOOL</span><br>Completed my class 10th Education
                            with 93.6% marks.</li>
                        <li><span>SRI CHAITANYA TECHNO SCHOOL</span><br>Completed my class 12th Education
                            with 95.6%marks.</li>
                        <li><span>CV RAMAN GLOBAL UNIVERSITY</span><br>Currently pursuing B.tech in Computer Science and Engineering.<br></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>
<!-- -----------------------services---------------------------- -->
<div id="services">
    <div class="container">
        <h1 class="subtitle">My Services</h1>
        <div class="services-list">
            <div>
                <i class="fa-solid fa-code"></i>
                <!-- web-development icon -->
                <h2>WEB-DEVELOPMENT</h2><br>
                <p>Web development is the building and maintenance of websites, it's the work that happens behind
                    the scenes to make a website look great, work fast and perform well with a seamless user
                    experience. Web developers, or 'devs', do this by using a variety of coding languages.</p>
                <a href="https://www.geeksforgeeks.org/web-development/">Learn more</a>
            </div>
            <div>
                <i class="fa-brands fa-java"></i>
                <!-- Java icon -->
                <h2>JAVA</h2><br>
                <p>Java is a widely used object-oriented programming language and software platform that runs on
                    billions of devices, including notebook computers, mobile devices, gaming consoles, medical
                    devices and many others. The rules and syntax of Java are based on the C and C++ languages.</p>
                <a
                    href="https://www.geeksforgeeks.org/java/.">Learn
                    more</a>
            </div>
            <div>
                <i class="fa-brands fa-codepen"></i>
                <!-- DSA icon -->
                <h2>DSA</h2><br>
                <p>A data structure is a storage that is used to store and organize data. It is a way of arranging
                    data on a computer so that it can be accessed and updated efficiently.</p>
                <a href="https://www.geeksforgeeks.org/data-structures/">Learn more</a>
            </div>

        </div>
    </div>
</div>
<!-- ----------------------portfolio------------------ -->
<div id="projects">
    <div class="container">
        <h1 class="subtitle">My Work</h1>
         
        <div class="work-list">
            <div class="work">
               
               <img src="image.jpg">
                <div class="layer">
                    <h3>Temperature Converter Web Application</h3><br />
                    <p>A temperature converter helps in the conversion of the measurement units of the temperature
                        recorded in a particular unit.</p>
                    <a href="https://github.com/Varshajha5/TEMPERATUREconverter"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="https://wallpapercave.com/wp/wp8984777.png"
                    height="280px">
                <div class="layer">
                    <h3>TIC TAC TOE game web application</h3><br />
                    <p>TIC-TAC-TOE is a game in which two players take turns in drawing either an 'O' or an 'X' in one square of a grid consisting of nine squares.</p>
                    <a href="https://github.com/Varshajha5/TIC_TAC_TOE_GAME/tree/main"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="calimg.png" height="280px">
                <div class="layer">
                    <h3>SIMPLE CALCULATOR Web Application</h3><br/>
                    <p>Calculator Web Application is the application used for performing basic mathematical operations like Addition,Subtraction,Multiplication & Divisions.</p>
                    <a href="https://github.com/Varshajha5/SIMPLECALCULATOR"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>

        </div>
        <a href="https://github.com/Varshajha5" class="btn">See more</a>

    </div>
</div>
<!-- ---------------------------contacts------------------------ -->
<div id="contact">
    <div class="container">
        <div class="row">
            <!-- for left column -->
            <div class="contact-left">
                <h1 class="sub-titles">Contact Me</h1>
                <p><i class="fa-solid fa-paper-plane"></i>jhavarsha482@gmail.com</p>
                <p><i class="fa-solid fa-phone"></i></p>
              
                
                <a href="RESUMEvkj.pdf" download class="btn btn2">Download CV</a>
                <!-- whenever we will cick Down...,it will start downloading -->
            </div>
            <!-- creating form for right column-->
            <div class="contact-right">
                <form name="submit-to-google-sheet">
                    <!-- the form name will be same as we have used for in JS (last-part) -->
                    <input type="text" name="Name" placeholder="Your Name" required>
                    <input type="email" name="Email" placeholder="Your Email" required>
                    <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                    <button type="submit" class="btn btn2">Submit</button>

                </form>
                <span id="msg"></span>
            </div>
        </div>

    </div>
    <div class="copy-right">
        <p>Copyright @ Varsha 2023.</p>
    </div>
</div>


</script>
 
</body>

</html>

<script type="text/javascript" src="script.js"></script>
    
</body>
</html>

//CSS CODE

      *{
            margin:0;
            padding:0;
        }
        body{
        background-color:rgb(0,0,33);
        color:white;
        font-family: 'Poppins', sans-serif;
        }
        nav{
            display: flex;
            justify-content: space-around;
            align-items:center;
            height: 70px;
            background-color: rgb(42, 42, 214);
        }
        nav ul{
            display: flex;
            justify-content: center;
        }
        nav ul li{
            list-style:none;
            margin:0 23px;
        }

        nav ul li a{
            text-decoration: none;
            color:white;
        }
        nav ul li :hover{
            color:rgb(209, 46, 204);
            font: size 1.04rem;
        }
        main hr
        {
            border:0;
            background: #9c97f1;
            height:1.2px;
            margin:40px 84px;

        }
        .left{
            font-size:1.5rem;
        }
        .firstSection{
            display: flex;
            justify-content: space-around;
            align-items:center;
            margin: 140px 0;


            
        }

        .firstSection > div{ 
            width:40%;
        }
        .leftSection{
            font-size: 3rem;
            margin:70px 0;

        }
        .rightSection img{
            
            width: 80%;
            margin: 50px 0;
        

        }
        .purple{
            color:rgb(225, 31, 250);
        }
        .text-gray
        {
            color:gray;
        }

        #element {
            color:rgb("170,107,228");

        }
        .secondSection
        {
            max-width:80vw;
            margin:auto;
            height:80vh;

        }

        .secondSection h1{
            font-size:1.9rem;
        }

        .secondSection .box {
            background: white;
            width:80vw;
            height: 3px;
            margin:56px 0;
            display: flex;
        }
        .secondSection .vertical{
            height:100px;
            width:1px;
            background-color: white;
            margin:0 100px;
        }
        .image-top{
            width: 23px;
            position:relative;
            top: -32px;
            left: -9px;
        }

        .vertical-title{
            position:relative;
            top:75px;
            width:150px;

        }
        .vertical-desc{
            position:relative;
            top:86px;
            color:gray;
            width:150px;
            font-size:9px;

        }


    
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    /* font-family: 'Poppins',sans-serif; */
    font-family: 'Roboto', sans-serif;
}
html{
    scroll-behavior: smooth;
}
body{
    background-color: black;
}
#header{ 
     width: auto;
    
}
.container{
    padding: 10px 10%;
}
nav{
    display: flex;
    align-items: center;
    justify-content:space-between;
    flex-wrap: wrap;
}
.logo{
    width: 140px;
}
nav ul li{
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
    
}
nav ul li a{
    text-decoration: none;
    color: white;
    font-size: 25px;
    position: relative;
}
nav ul li a::after{
   content: '';
   width: 0%;
   height: 3px;
   background:red;
   position: absolute;
   left: 0;
   bottom: -6px; 
}
nav ul li a:hover::after{
    width: 100%;
}
.header-text{
    margin-top: 10%;
    font-size: 30px;
    color: white;
}
/*----------------------------------for type writting effect--------------------------------*/
.header-text  h1{
    margin-top: 5%;
    font-size:  60px;
    width: 0ch; /*it means it will start from 0 character*/
    overflow: hidden;
    white-space: nowrap;
    animation: text 3s steps(44) infinite;
    border-right: 3px solid red;

}
@keyframes text {
    0% {
        width: 0ch;
    }
    50% {
        width: 20ch;
    }
    
}
.header-text  h1 span{
    color:red;
}
.header-text p{
    font-size:40px;
}





/* ---------------------------ABOUT------------------------ */
#about{
    padding: 100px 0px;
    color: white;
}
.row{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}
.about-col-1{
    flex-basis: 35%;
}
.about-col-1 img{
    width: auto;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
    padding-left: 35px;
}
.subtitle{
    font-size:60px;
    font-weight: 900;
    color: white;
}
 p{
    line-height: 1.5em;
}
.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}
.tab-links{
    margin-right: 50px;
    font-size:18px;
    font-weight: 800;
    cursor: pointer;
    position: relative;
}
.tab-links::after{
    content: "";
    width: 0;
    height: 3px;
    background-color:red;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition:0.5 seconds; 
}
.tab-links.active-link::after{
    width: 50%;
}
.tab-contents ul li{
    list-style: none;
    margin:10px 0;

}
.tab-contents ul li span{
    color:rgba(255, 0, 0, 0.85);
    font-size:14px;

}
.tab-contents{
    display:none; /*it will hide all the contents under skills,Achievements,education*/
}
.tab-contents.active-tab{
    display:block; /*it will display the content of skills part*/
}

/* -------------------services--------------------------------------- */
#services{
    padding:130px 0;
}
.services-list{
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
    grid-gap: 40px;
    margin-top: 50px;
    color: white;
    transition: background 0.5s, transform 0.5s;
    
}
.services-list div{
    background:rgba(128, 128, 128, 0.208);
    padding:40px;
    font-size: 13px;
    font-weight: 300px;
    border-radius: 10px;
    
}
.services-list div i{
    font-size: 50px;
    margin-bottom: 30px;

}
.services-list div h2{
    font-size:30px;
    font-weight: 500;
    margin-bottom:15px;
}
.services-list div a{
    text-decoration: none;
    color: white;
    font-size:12px;
    margin-top: 20px;
    display: inline-block;
}
.services-list :hover{
    background:rgba(255, 8, 0, 0.986);
    transform:translateY(-10px) /*it will move the box by 10 px*/

}
/* ----------------------portfolio-------------------- */


.work-list{
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
    grid-gap: 40px;
    margin-top: 50px;
    
    
}
.work{
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}
.work img{
    border-radius: 10px;
    float: left;
    width: 100%;
    padding:5px;
    transition: transform 0.5s; /*it will zoom in the image*/
}
.layer{
    color: white;
    width: 100%;
    height: 0;
    background:linear-gradient(rgba(0,0,0,0.6),#ff004f);
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 20px;
    text-align: center;
    font-size: 14px;
    transition: height 0.5s;
}
.layer h3{
    font-weight: 500px;
    margin-bottom: 20px;

}
.layer a{
    margin-top: 20px;
    color: #ff004f;
    text-decoration: none;
    font-size: 18px;
    line-height: 60px;
    background: #fff;
    width: 60px;
    height: 60px;
    border-radius:50%;
    text-align: center;
}
.work:hover img {
    transform: scale(1.1);  /*it will zoom in the background images*/
}
.work:hover .layer{
    height: 100%;

}
.btn{
    display: block;
    margin: 50px auto;
    width: fit-content;
    border: 1px solid #ff004f;
    padding: 14px 50px;
    border-radius: 6px;
    text-decoration: none;
    color: #fff;
    transition background:0.5s;
}
.btn:hover{
    background:red;
}
/* -------------------------contact---------------- */
#contact{
    padding:10px 0;}
.contact-left .sub-titles{
    color: white;
    font-size: 60px;
}
p{
    color: white;
}
.contact-right{
    flex-basis: 65%;
}
.contact-left p{
    margin-top:30px;
}
.contact-left p i{
    color:rgba(255, 0, 0, 0.463);
    margin-right: 15px;
    font-size: 25px;
}
.social-icons{
    margin-top:30px;

}
.social-icons a{
    text-decoration:none;
    font-size:30px;
    margin-right: 15px;
    color: white;
    display: inline-block;
    transition: transform 0.5s;
}
.social-icons a:hover{
    color: #ff004f;
    transform: translateY(-5px); /*it will move up and the color will change*/

}
.btn.btn2{
    display: inline-block;
    background: #ff004f;
}

/* for right column contact name table  */
.contact-right form{
    width: 110%;

}
form input,form textarea{
    width: 100%;
    border: 0;
    outline: none;
    background: #262626;
    padding: 15px;
    margin: 15px 0;
    color: #fff;
    font-size:18px;
    border-radius:6px;
    
}
form .btn2{
    padding: 14px 60px;
    font-size:18px;
    margin-top:20px;
    /* cursor: pointer; */
}
.copy-right{
    width: 100%;
    text-align: center;
    padding:25px 0;
    background-color:#262626;
    font-weight: 300;
    margin-top: 20px;
}


.fa-solid{
    display: none;
}

   //js code
   var tablinks = document.getElementsByClassName("tab-links");
var tabcontents = document.getElementsByClassName("tab-contents");
// -----------------------logic for ABOUT section---------------
function opentab(tabname) {
    for(tablink of tablinks) {
        tablink.classList.remove("active-link");
    }
    for (tabcontent of tabcontents) {
        tabcontent.classList.remove("active-tab");
    }
    event.currentTarget.classList.add("active-link");
    document.getElementById(tabname).classList.add("active-tab"); //it will take one of the three id at a time from the function opentab and display it
}
// ------------------------for sidemenu( for responsive)--------------
var sidemenu=document.getElementById("sidemenu");
function openmenu(){
    sidemenu.style.right="0";
}
function closemenu(){
    sidemenu.style.right="-200px";
}
// ---------------------making the form work for everyone whoever gives any input-----
const scriptURL = 'https://forms.gle/FZDpxxrnRsSfSD498'
        const form = document.forms['submit-to-google-sheet']
        const msg = document.getElementById("msg")

        form.addEventListener('submit', e => {
            e.preventDefault()
            fetch(scriptURL, { method: 'POST', body: new FormData(form) })
                .then(response => {
                    msg.innerHTML = "Message sent successfully!";
                    setTimeout(function () {
                        msg.innerHTML = "";
                    }, 5000)
                    form.reset();
                })
                .catch(error => console.error('Error!', error.message))
        })

