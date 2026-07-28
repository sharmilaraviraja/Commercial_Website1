# Ex02 Commercial Website
## Date:27.07.2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
HTML

<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>NovaCraft Studio</title>

<link rel="stylesheet" href="style.css">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

</head>


<body>


<header>

<nav>

<h2 class="logo">NovaCraft ✦</h2>


<ul>

<li><a href="#">Home</a></li>
<li><a href="#">Services</a></li>
<li><a href="#">Projects</a></li>
<li><a href="#">Contact</a></li>

</ul>


<a class="btn" href="#">Start Project</a>


</nav>

</header>




<!-- Hero Section -->


<section class="hero">


<div class="hero-text">

<h1>
Create
<span>Digital Experiences</span>
That Inspire
</h1>


<p>
We design modern websites, mobile apps and
creative digital products for businesses.
</p>


<a class="main-btn" href="#">
Explore Services
</a>


</div>




<div class="visual">


<div class="glass-box">

<i class="fa-solid fa-code"></i>

<h3>
Web Development
</h3>

<p>
Modern responsive websites
</p>

</div>



<div class="glass-box second">

<i class="fa-solid fa-palette"></i>

<h3>
UI/UX Design
</h3>

<p>
Beautiful user experiences
</p>

</div>


</div>


</section>






<!-- Services -->


<section class="services">


<h2>Our Services</h2>


<div class="service-container">



<div class="card">

<i class="fa-solid fa-globe"></i>

<h3>
Website Design
</h3>

<p>
Creative and responsive websites.
</p>

</div>



<div class="card">

<i class="fa-solid fa-mobile"></i>

<h3>
Mobile Apps
</h3>

<p>
Powerful mobile applications.
</p>

</div>



<div class="card">

<i class="fa-solid fa-lightbulb"></i>

<h3>
Brand Ideas
</h3>

<p>
Unique digital strategies.
</p>

</div>



</div>


</section>







<!-- Projects -->


<section class="projects">


<h2>Featured Projects</h2>


<div class="project-container">


<div class="project">

<h3>
E-Commerce
</h3>

<p>
Online shopping platform
</p>

</div>



<div class="project">

<h3>
AI Dashboard
</h3>

<p>
Smart analytics system
</p>

</div>



<div class="project">

<h3>
Portfolio
</h3>

<p>
Personal branding website
</p>

</div>


</div>


</section>







<!-- Pricing -->


<section class="pricing">


<h2>
Simple Pricing
</h2>


<div class="price">


<h3>
Starter
</h3>


<h1>
£99
</h1>


<p>
✔ Landing Page<br>
✔ Responsive Design<br>
✔ Basic SEO
</p>


<a href="#">
Choose Plan
</a>


</div>


</section>







<!-- Contact -->


<section class="contact">


<h2>
Let's Build Something Amazing 🚀
</h2>


<form>


<input type="text" placeholder="Name">


<input type="email" placeholder="Email">


<textarea placeholder="Message"></textarea>


<button>
Send Message
</button>


</form>


</section>






<footer>

<p>
© 2026 NovaCraft Studio
</p>

</footer>



</body>

</html>

CSS
*{

margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,Arial;

}



body{

color:white;

background:

linear-gradient(
135deg,
#0f172a,
#4c1d95,
#0284c7
);

}



/* NAVBAR */


header{

padding:25px 8%;

}


nav{

display:flex;

justify-content:space-between;

align-items:center;


background:
rgba(255,255,255,0.15);


backdrop-filter:blur(20px);


padding:20px;

border-radius:25px;

}



.logo{

font-size:28px;

}



ul{

display:flex;

gap:35px;

list-style:none;

}



a{

color:white;

text-decoration:none;

}



.btn,
.main-btn{

background:
rgba(255,255,255,0.2);

padding:12px 25px;

border-radius:30px;

}





/* HERO */


.hero{

display:flex;

justify-content:space-between;

align-items:center;

padding:80px 8%;

}



.hero-text{

width:50%;

}



.hero-text h1{

font-size:55px;

}



.hero-text span{

color:#38bdf8;

}



.hero-text p{

font-size:18px;

margin:25px 0;

}



.visual{

display:flex;

flex-direction:column;

gap:30px;

}



.glass-box{

width:300px;

padding:35px;


background:
rgba(255,255,255,0.15);


backdrop-filter:blur(15px);


border-radius:25px;


transition:.4s;

}



.glass-box:hover{

transform:translateY(-15px);

}



.glass-box i{

font-size:40px;

color:#38bdf8;

}




/* COMMON */


section{

padding:70px 8%;

}


h2{

text-align:center;

font-size:40px;

margin-bottom:40px;

}




/* SERVICES */


.service-container{

display:flex;

justify-content:center;

gap:30px;

}



.card{

width:300px;

padding:35px;


background:
rgba(255,255,255,0.15);


border-radius:25px;


transition:.3s;

}



.card:hover{

transform:scale(1.05);

}



.card i{

font-size:40px;

color:#38bdf8;

}





/* PROJECT */


.project-container{

display:flex;

gap:30px;

justify-content:center;

}



.project{

width:300px;

padding:35px;


background:
rgba(255,255,255,0.15);


border-radius:25px;

}





/* PRICE */


.price{

width:350px;

margin:auto;

text-align:center;


background:
rgba(255,255,255,0.15);


padding:40px;

border-radius:30px;

}



.price h1{

font-size:50px;

}





/* CONTACT */


form{

display:flex;

flex-direction:column;

align-items:center;

gap:15px;

}



input,
textarea{


width:350px;

padding:15px;

border:none;

border-radius:15px;


background:
rgba(255,255,255,0.2);


color:white;

}



textarea{

height:120px;

}



button{

padding:15px 35px;

border-radius:30px;

border:none;

cursor:pointer;

}




footer{

text-align:center;

padding:30px;

}




/* MOBILE RESPONSIVE */


@media(max-width:768px){


nav,
.hero,
.service-container,
.project-container{

flex-direction:column;

gap:30px;

}



.hero-text{

width:100%;

}


.hero-text h1{

font-size:40px;

}


}
```

## OUTPUT
<img width="1882" height="900" alt="Screenshot 2026-07-28 140331" src="https://github.com/user-attachments/assets/ba6fc3a7-b5d5-497a-bd47-d417eb3f7897" />
<img width="1875" height="887" alt="Screenshot 2026-07-28 140352" src="https://github.com/user-attachments/assets/e2e57cda-34f5-4ff4-97de-f4be3b43bb54" />
<img width="1733" height="857" alt="Screenshot 2026-07-28 140424" src="https://github.com/user-attachments/assets/3a91ecdb-a4e2-4eb8-8df8-b7521a764bf8" />
<img width="1252" height="820" alt="Screenshot 2026-07-28 140435" src="https://github.com/user-attachments/assets/342e3ac4-dc98-4d31-b499-ef00460034f2" />



## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
