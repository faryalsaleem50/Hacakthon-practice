# Hacakthon-practice

<!DOCTYPE html>

<html lang="en">

<head>

 <meta charset="UTF-8">

 <meta name="viewport" content="width=device-width, initial-scale=1">

 <title>School Heart</title>

 <!-- FontAwesome for social icons -->

 <link

 rel="stylesheet"

 href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"

 

integrity="sha512-k6RqeWeci5ZR/Lv4MR0sA0FfDOMQj1Q6H9q9R5O3tvZJRoIh1Q

p+5l5z0PRwKMp7QfZe1GjQ1lU6h0l+8f+5g=="

 crossorigin="anonymous"

 referrerpolicy="no-referrer" />

 <style>

 * { margin:0; padding:0; box-sizing:border-box; }

 body { font-family:Arial,sans-serif; color:#333; line-height:1.6; }

 /* Navbar */

 header { background:#004080; padding:15px 0; }

 .navbar { max-width:1200px; margin:0 auto; display:flex;

justify-content:space-between; align-items:center; }

 .navbar .logo { color:#fff; font-size:24px; font-weight:bold; }

 .navbar .nav-links { list-style:none; display:flex; }
   .navbar .nav-links li { margin-left:20px; }

 .navbar .nav-links a { color:#fff; text-decoration:none; font-size:16px; }

 /* Hero */

 #hero { position:relative; height:90vh; display:flex; justify-content:center;

align-items:center; text-align:center; color:#010101; }

 #hero::before {

 content:""; position:absolute; top:0; left:0; width:100%; height:100%;

 

background:url('https://cdn.dribbble.com/userupload/10092966/file/original-b8893c72

ca3804613ffba3bae7b048b9.jpg') no-repeat center/cover;

 opacity:0.7; z-index:-1;

 }

 #hero h1 { font-size:48px; background:rgba(0,0,0,0.5); padding:20px 30px;

border-radius:8px; } br

 #hero h2 {font-size: 30px; background-color: violet rgba(0,0,0,0.5); padding: 20px

30px; border-radius: 8px;}

 /* About */

 section { padding:60px 20px; }

 #about { background:#f2f2f2; }

 #about h2 { text-align:center; font-size:32px; color:#004080; margin-bottom:30px; }

 .about-content { max-width:1000px; margin:0 auto; display:flex; flex-wrap:wrap;

gap:20px; align-items:center; }

 .about-content img { width:300px; border-radius:10px; }

 .about-text { flex:1; min-width:300px; }

 /* Books */

 #books { background:#fff; }
   #books h2 { text-align:center; font-size:32px; color:#004080; margin-bottom:30px;

}

 .book-list { display:flex; flex-wrap:wrap; justify-content:center; gap:30px; }

 .book-item { background:#f9f9f9; width:280px; border-radius:10px;

overflow:hidden; box-shadow:0 4px 10px rgba(0,0,0,0.1); transition:transform .3s; }

 .book-item img { width:100%; height:180px; object-fit:cover; }

 .book-item h3 { margin:15px; font-size:20px; color:#004080; }

 .book-item p { margin:0 15px 15px; font-weight:bold; color:#0073e6; }

 .book-item:hover { transform:translateY(-8px); }

 /* Popular Teacher */

 #teacher { background:#f2f2f2; }

 #teacher h2 { text-align:center; font-size:32px; color:#004080;

margin-bottom:30px; }

 .teacher-content { max-width:1000px; margin:0 auto; display:flex; flex-wrap:wrap;

gap:30px; align-items:center; justify-content:center; }

 .teacher-content img { width:300px; height:300px; border-radius:50%;

object-fit:cover; }

 .teacher-text { flex:1; min-width:300px; }

 .teacher-text p { font-size:18px; margin-bottom:20px; }

 .teacher-text video { width:100%; border-radius:10px; }

 /* Popular Courses */

 #courses { background:#fff; }

 #courses h2 { text-align:center; font-size:36px; color:#004080;

margin-bottom:40px; }

 .course-container { display:flex; flex-wrap:wrap; justify-content:center; gap:30px;

margin-bottom:50px; }

 .course-card { background:#fff; width:300px; border-radius:10px; overflow:hidden;

box-shadow:0 4px 10px rgba(0,0,0,0.1); transition:transform .3s; }

 .course-card img { width:100%; height:200px; object-fit:cover; }
   .course-card h3 { margin:15px; font-size:22px; }

 .course-card p { margin:0 15px 15px; font-weight:bold; color:#0073e6; }

 .course-card:hover { transform:translateY(-10px); }

 .search-bar { max-width:600px; margin:0 auto; display:flex; gap:10px; }

 .search-bar input {

 flex:1; padding:15px 20px; font-size:18px; border:2px solid #004080;

border-radius:50px; outline:none; transition:border-color .3s, transform .3s;

 }

 .search-bar input:focus { border-color:#0073e6; transform:scale(1.02); }

 .search-bar button {

 padding:15px 30px; background:#004080; color:#fff; border:none;

border-radius:50px; font-size:18px; cursor:pointer; transition:background .3s;

 }

 .search-bar button:hover { background:#0073e6; }

 /* Contact */

 #contact { background:#fff; }

 #contact h2 { text-align:center; font-size:32px; color:#004080;

margin-bottom:30px; }

 .contact-form { max-width:500px; margin:0 auto; display:flex; flex-direction:column;

gap:15px; }

 .contact-form input,

 .contact-form textarea {

 padding:15px; border:1px solid #ccc; border-radius:5px;

 }

 .contact-form button {

 background:#004080; color:#fff; padding:12px; border:none; border-radius:5px;

font-size:18px; cursor:pointer; transition:background .3s;
   .contact-form button:hover { background:#0073e6; }

 /* Footer */

 footer { background:#004080; color:#fff; text-align:center; padding:30px 20px; }

 .social-icons { margin:15px 0; }

 .social-icons a { color:#fff; font-size:24px; margin:0 10px; transition:color .3s; }

 .social-icons a:hover { color:#ffcc00; }

 /* Responsive */

 @media (max-width:768px) {

 .about-content,

 .teacher-content,

 .book-list,

 .course-container { flex-direction:column; align-items:center; }

 .search-bar { flex-direction:column; }

 .search-bar button { width:100%; }

 }

 </style>

</head>

<body>

 <!-- Navbar -->

 <header>

 <div class="navbar">

 <div class="logo">School Heart</div>

 <ul class="nav-links">

 <li><a href="#hero">Home</a></li>

 <li><a href="#about">About</a></li>
 <li><a href="#books">Books</a></li>

 <li><a href="#teacher">Teacher</a></li>

 <li><a href="#courses">Courses</a></li>

 <li><a href="#contact">Contact</a></li>

 </ul>

 </div>

 </header>

 <!-- Hero -->

 <section id="hero">

 <h1>Welcome to School Heart <br>

 our goal is to make online education everywehere</h1>

 </section>

 <!-- About -->

 </div>

 </section>

 <!-- Books -->

 <section id="books">

 <h2>Our Books</h2>

 <div class="book-list">

 <div class="book-item">

 <img

src="https://accountscoaching.com/wp-content/uploads/elementor/thumbs/Mathemat

ics-Banner-qj69wgy3eiwz8wi0ebvw35m3fqboqmna8yurbu8a9s.webp"

alt="Mathematics">

 <h3>Mathematics</h3><p>$2</p>

 </div>
 <div class="book-item">

 <img

src="https://images.unsplash.com/photo-1568605114967-8130f3a36994?auto=forma

t&fit=crop&w=400&q=80" alt="Science">

 <h3>Science</h3><p>$2</p>

 </div>

 <div class="book-item">

 <img

src="https://images.unsplash.com/photo-1521587760476-6c12a4b040da?auto=form

at&fit=crop&w=400&q=80" alt="History">

 <h3>History</h3><p>$2</p>

 </div>

 </div>

 </section>

 <!-- Popular Teacher -->

 <section id="teacher">

 <h2>Popular Teacher</h2>

 <div class="teacher-content">

 <img

src="https://res.cloudinary.com/ybmedia/image/upload/c_crop,h_1320,w_2000,x_0,y

_0/c_scale,f_auto,q_auto,w_700/v1/m/0/a/0aaa7c8fc51231ee41e08d7914c03e3105

35030d/sister-mary-clarence-sister-act-2-back-habit.jpg" alt="Teacher">

 <div class="teacher-text">

 <p>Dr. Aisha Khan has over 15 years of experience and is beloved by her

students for her interactive teaching style.</p>

 <video controls>

 <source src="https://youtu.be/7wnove7K-ZQ?t=6" type="video/mp4">

 </video>

 </div>

 </div>
 </section>

 <!-- Popular Courses & Search -->

 <section id="courses">

 <h2>Our Popular Courses</h2>

 <div class="course-container">

 <div class="course-card">

 <img

src="https://www.learncomputerscienceonline.com/wp-content/uploads/2022/07/Intro

duction-To-Computer-Science-Beginners-Guide-To-Computer-Science-CS-CS-Major

-Computer-Science.jpg" alt="Computer Science">

 <h3>Computer Science</h3><p>$15</p>

 </div>

 <div class="course-card">

 <img

src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRMJBWCa1FxtBgBh

RWDWM2OGn6Jyp1QmRgPiQ&s" alt="Art">

 <h3>graphic designing</h3><p>$10</p>

 </div>

 <div class="course-card">

 <img

src="https://miro.medium.com/v2/resize:fit:1200/1*V-Jp13LvtVc2IiY2fp4qYw.jpeg"

alt="Music">

 <h3>web development</h3><p>$12</p>

 </div>

 </div>

 <div class="search-bar">

 <input type="text" placeholder="Search Courses...">

 <button>Search</button>
 </div>

 </section>

 <!-- Contact -->

 <section id="contact">

 <h2>Contact Us</h2>

 <div class="contact-form">

 <input type="text" placeholder="Your Name">

 <input type="email" placeholder="Your Email">

 <textarea rows="5" placeholder="Your Message"></textarea>

 <button>Send Message</button>

 </div>

 <section id="about">

 <h2>About Us</h2>

 <div class="about-content">

 <img

src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR1-9V8vro2Ofb_tCia

HwU7FyPGr06a6PSXJQ&s" alt="About">

 <div class="about-text">

 <p>We inspire young minds with quality education and innovative teaching.

Our mission is to empower every student to reach their potential.</p>

 </div>

 </section>

 <!-- Footer -->

 <footer>

 <p>School Heart © 2025</p>

 <div class="social-icons">

 <a href="#"><i class="fab fa-facebook-f"></i></a>
 <a href="#"><i class="fab fa-twitter"></i></a>

 <a href="#"><i class="fab fa-google"></i></a>

 </div>

 </footer>

</body>

</html>
 
 
