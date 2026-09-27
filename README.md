# TIT-senior-secondary-school-Bhiwani-
Welcome to TIT senior secondary school Bhiwani, inspiring minds, building futures
T.I.T. SR. SEC. SCHOOL, BHIWANI
Complete Website Source Code
index.html — HTML + CSS + JavaScript
The complete website source code is provided below. Keep the accompanying images folder in the same directory as index.html for the website photographs and logo to work.
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="description" content="T.I.T. Senior Secondary School, Bhiwani, Haryana — academics, technology, practical learning, sports and student activities.">
<meta name="theme-color" content="#0b3b66">
<title>T.I.T. Senior Secondary School, Bhiwani | Official Website</title>
<style>
:root{--navy:#082f55;--blue:#0b5fa5;--sky:#eaf5ff;--gold:#f4b400;--ink:#17212b;--muted:#607080;--white:#fff;--line:#dce6ef;--shadow:0 18px 50px rgba(8,47,85,.12)}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",Arial,sans-serif;color:var(--ink);background:#fff;line-height:1.65}
img{max-width:100%;display:block}
a{text-decoration:none;color:inherit}
button,input,select,textarea{font:inherit}
.container{width:min(1180px,92%);margin:auto}
.topbar{background:var(--navy);color:#eaf4ff;font-size:13px}
.topbar .container{display:flex;justify-content:space-between;gap:15px;flex-wrap:wrap;padding:8px 0}
header{position:sticky;top:0;z-index:50;background:rgba(255,255,255,.96);backdrop-filter:blur(12px);box-shadow:0 2px 18px rgba(0,0,0,.08)}
.nav{height:76px;display:flex;align-items:center;justify-content:space-between;gap:20px}
.brand{display:flex;align-items:center;gap:12px}
.brand img{width:55px;height:55px;object-fit:contain;border-radius:50%}
.brand strong{display:block;color:var(--navy);font-size:18px;line-height:1.15}
.brand span{font-size:11px;color:var(--muted)}
nav{display:flex;align-items:center;gap:19px}
nav a{font-size:14px;font-weight:750;color:#263746}
nav a:hover{color:var(--blue)}
.menu{display:none;border:0;background:none;font-size:29px;color:var(--navy);cursor:pointer}
.btn{display:inline-flex;align-items:center;justify-content:center;gap:8px;border:0;border-radius:10px;padding:12px 19px;font-weight:800;cursor:pointer;transition:.2s}
.btn:hover{transform:translateY(-2px)}
.btn-gold{background:var(--gold);color:#18242f}
.btn-blue{background:var(--blue);color:#fff}
.btn-light{background:#fff;color:var(--navy)}
.btn-outline{border:1px solid rgba(255,255,255,.7);color:#fff;background:transparent}
.hero{position:relative;min-height:610px;display:flex;align-items:center;color:#fff;overflow:hidden;background:var(--navy)}
.hero:before{content:"";position:absolute;inset:0;background:linear-gradient(90deg,rgba(4,28,50,.93) 0%,rgba(4,28,50,.72) 48%,rgba(4,28,50,.18) 100%),url("images/school-photo-01.jpg") center/cover}
.hero-content{position:relative;padding:75px 0;max-width:790px}
.kicker{display:inline-block;background:rgba(244,180,0,.95);color:#14202b;border-radius:999px;padding:7px 14px;font-size:13px;font-weight:900;margin-bottom:17px}
.hero h1{font-size:clamp(38px,6vw,68px);line-height:1.02;letter-spacing:-1.5px;margin-bottom:20px}
.hero p{font-size:18px;color:#e7f0f8;max-width:690px;margin-bottom:27px}
.hero-actions{display:flex;gap:10px;flex-wrap:wrap}
section{padding:82px 0}
.section-head{text-align:center;max-width:780px;margin:0 auto 42px}
.section-head .eyebrow{color:var(--blue);font-weight:900;font-size:13px;text-transform:uppercase;letter-spacing:1.2px}
.section-head h2{color:var(--navy);font-size:clamp(29px,4vw,42px);line-height:1.15;margin:8px 0 12px}
.section-head p{color:var(--muted)}
.intro{background:var(--sky)}
.about-grid{display:grid;grid-template-columns:1.05fr .95fr;gap:48px;align-items:center}
.photo-card{border-radius:22px;overflow:hidden;box-shadow:var(--shadow);background:#fff}
.photo-card img{width:100%;height:420px;object-fit:cover}
.about-copy h3{font-size:29px;color:var(--navy);margin-bottom:12px}
.about-copy p{color:#506172;margin-bottom:17px}
.checks{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:20px}
.check{background:#fff;border:1px solid var(--line);padding:13px 14px;border-radius:12px;font-weight:750}
.check b{color:#148447;margin-right:7px}
.cards{display:grid;grid-template-columns:repeat(3,1fr);gap:20px}
.card{background:#fff;border:1px solid var(--line);border-radius:17px;padding:25px;box-shadow:0 8px 30px rgba(8,47,85,.06);transition:.2s}
.card:hover{transform:translateY(-4px);box-shadow:var(--shadow)}
.card .icon{font-size:31px;margin-bottom:11px}
.card h3{color:var(--navy);margin-bottom:7px}
.card p{color:var(--muted)}
.dark{background:var(--navy);color:#fff}
.dark .section-head h2{color:#fff}
.dark .section-head p{color:#c9d8e5}
.stats{display:grid;grid-template-columns:repeat(4,1fr);gap:18px}
.stat{text-align:center;padding:22px;border:1px solid rgba(255,255,255,.12);border-radius:16px;background:rgba(255,255,255,.06)}
.stat strong{display:block;font-size:39px;color:var(--gold);line-height:1.1}
.stat span{font-size:14px;color:#d7e4ee}
.programs .card{min-height:190px}
.gallery{display:grid;grid-template-columns:repeat(4,1fr);gap:13px}
.gallery figure{position:relative;border-radius:14px;overflow:hidden;cursor:pointer;background:#ddd;min-height:180px}
.gallery img{width:100%;height:220px;object-fit:cover;transition:.35s}
.gallery figure:hover img{transform:scale(1.05)}
.gallery figcaption{position:absolute;left:10px;right:10px;bottom:10px;background:rgba(4,28,50,.78);color:#fff;border-radius:9px;padding:7px 10px;font-size:12px;font-weight:700}
.facility-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px}
.facility{display:flex;gap:14px;align-items:flex-start;padding:21px;border:1px solid var(--line);border-radius:15px;background:#fff}
.facility .icon{font-size:28px}
.notice-wrap{display:grid;grid-template-columns:1.1fr .9fr;gap:22px}
.notice-box{background:#fff;border-radius:17px;padding:25px;border:1px solid var(--line);box-shadow:0 8px 30px rgba(8,47,85,.06)}
.notice-box h3{color:var(--navy);margin-bottom:12px}
.notice-box li{list-style:none;padding:12px 0;border-bottom:1px solid var(--line)}
.notice-box li:last-child{border-bottom:0}
.notice-box time{display:block;font-size:11px;color:var(--blue);font-weight:800}
.cta{background:linear-gradient(120deg,var(--blue),var(--navy));color:#fff;text-align:center}
.cta h2{font-size:39px;margin-bottom:10px}
.cta p{color:#d9e9f6;margin-bottom:22px}
.staff{background:#f7fafc}
.staff-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:17px}
.staff-card{text-align:center;padding:22px;border-radius:15px;background:#fff;border:1px solid var(--line)}
.staff-avatar{width:65px;height:65px;margin:0 auto 11px;border-radius:50%;display:grid;place-items:center;background:var(--sky);font-size:28px}
.staff-card h3{font-size:16px;color:var(--navy)}
.staff-card p{font-size:13px;color:var(--muted)}
.contact-grid{display:grid;grid-template-columns:.8fr 1.2fr;gap:35px;align-items:start}
.contact-info{background:var(--navy);color:#fff;border-radius:20px;padding:30px}
.contact-info h3{font-size:25px;margin-bottom:9px}
.contact-item{padding:15px 0;border-bottom:1px solid rgba(255,255,255,.13)}
.contact-item:last-child{border-bottom:0}
.contact-item b{display:block;color:var(--gold);font-size:12px;text-transform:uppercase;letter-spacing:.7px}
form{background:#fff;border:1px solid var(--line);border-radius:20px;padding:30px;box-shadow:var(--shadow)}
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:15px}
label{font-size:13px;font-weight:800;color:#304253}
input,select,textarea{width:100%;margin-top:6px;border:1px solid #cfdbe5;border-radius:10px;padding:12px 13px;outline:none;background:#fff}
input:focus,select:focus,textarea:focus{border-color:var(--blue);box-shadow:0 0 0 3px rgba(11,95,165,.1)}
textarea{min-height:130px;resize:vertical}
.full{grid-column:1/-1}
.form-note{font-size:12px;color:var(--muted);margin-top:9px}
footer{background:#061e35;color:#c9d8e5;padding:45px 0 18px}
.footer-grid{display:grid;grid-template-columns:2fr 1fr 1fr 1.2fr;gap:30px}
footer h3{color:#fff;margin-bottom:12px}
footer ul{list-style:none}
footer li{margin:7px 0}
.footer-bottom{border-top:1px solid rgba(255,255,255,.12);margin-top:30px;padding-top:16px;text-align:center;font-size:12px}
.lightbox{position:fixed;inset:0;background:rgba(0,0,0,.9);z-index:100;display:none;align-items:center;justify-content:center;padding:20px}
.lightbox.open{display:flex}
.lightbox img{max-height:86vh;max-width:92vw;border-radius:10px}
.lb-close{position:absolute;top:16px;right:22px;color:#fff;background:none;border:0;font-size:38px;cursor:pointer}
.lb-caption{position:absolute;bottom:20px;color:#fff;background:rgba(0,0,0,.55);padding:8px 14px;border-radius:8px}
.toast{position:fixed;right:20px;bottom:20px;background:#102d45;color:#fff;padding:14px 18px;border-radius:10px;box-shadow:var(--shadow);display:none;z-index:120}
.to-top{position:fixed;right:20px;bottom:75px;width:43px;height:43px;border:0;border-radius:50%;background:var(--gold);color:#17212b;font-weight:900;display:none;cursor:pointer;z-index:40}
.reveal{opacity:0;transform:translateY(18px);transition:.6s}.reveal.show{opacity:1;transform:none}
@media(max-width:950px){
nav{display:none;position:absolute;left:0;right:0;top:76px;background:#fff;padding:18px;flex-direction:column;align-items:stretch;box-shadow:0 12px 25px rgba(0,0,0,.1)}
nav.open{display:flex}.menu{display:block}.cards{grid-template-columns:1fr 1fr}.staff-grid{grid-template-columns:1fr 1fr}.gallery{grid-template-columns:1fr 1fr}.facility-grid{grid-template-columns:1fr 1fr}.footer-grid{grid-template-columns:1fr 1fr}.about-grid,.notice-wrap,.contact-grid{grid-template-columns:1fr}.stats{grid-template-columns:1fr 1fr}
}
@media(max-width:560px){
.topbar .container{justify-content:center}.brand strong{font-size:14px}.brand span{font-size:9px}.hero{min-height:590px}.hero p{font-size:16px}.hero-content{padding:55px 0}.cards,.staff-grid,.gallery,.facility-grid,.footer-grid,.stats,.form-grid,.checks{grid-template-columns:1fr}.gallery img{height:210px}.photo-card img{height:300px}section{padding:60px 0}.cta h2{font-size:30px}
}
</style>
</head>
<body>
<div class="topbar"><div class="container"><span>📍 Bhiwani, Haryana</span><span>🎓 Learning • Technology • Sports • Values</span></div></div>
 
<header>
<div class="container nav">
<a class="brand" href="#home"><img src="images/school-logo.png" alt="T.I.T. Senior Secondary School logo"><div><strong>T.I.T. SENIOR SECONDARY SCHOOL</strong><span>Bhiwani, Haryana</span></div></a>
<button class="menu" id="menuBtn" aria-label="Open navigation">☰</button>
<nav id="nav">
<a href="#home">Home</a><a href="#about">About</a><a href="#academics">Academics</a><a href="#facilities">Facilities</a><a href="#activities">Activities</a><a href="#gallery">Gallery</a><a href="#contact">Contact</a><a class="btn btn-gold" href="#admission">Admissions</a>
</nav>
</div>
</header>
 
<main>
<section id="home" class="hero">
<div class="container hero-content">
<span class="kicker">WELCOME TO T.I.T. SENIOR SECONDARY SCHOOL</span>
<h1>Inspiring Minds.<br>Building Futures.</h1>
<p>A school environment where students learn with curiosity, develop practical skills, participate in sports and activities, and grow into confident and responsible citizens.</p>
<div class="hero-actions"><a class="btn btn-gold" href="#admission">Admission Enquiry →</a><a class="btn btn-outline" href="#gallery">View School Gallery</a></div>
</div>
</section>
 
<section id="about" class="intro">
<div class="container about-grid reveal">
<div class="photo-card"><img src="images/school-photo-02.jpg" alt="T.I.T. school event and students"></div>
<div class="about-copy">
<div class="section-head" style="text-align:left;margin:0 0 18px"><div class="eyebrow">About the School</div><h2>A learning community with a practical approach</h2></div>
<p>T.I.T. Senior Secondary School, Bhiwani provides students opportunities to learn through classroom teaching, laboratory work, computer education, projects, cultural activities and sports.</p>
<p>The school photographs featured on this website show real learning spaces, student activities, science demonstrations, computer education and school events.</p>
<div class="checks"><div class="check"><b>✓</b>Academic Learning</div><div class="check"><b>✓</b>Practical Education</div><div class="check"><b>✓</b>Technology & Coding</div><div class="check"><b>✓</b>Sports & Activities</div></div>
</div>
</div>
</section>
 
<section id="academics">
<div class="container">
<div class="section-head reveal"><div class="eyebrow">Academics</div><h2>Learning Beyond the Textbook</h2><p>Balanced learning that combines concepts, practice, creativity and digital skills.</p></div>
<div class="cards">
<div class="card reveal"><div class="icon">📚</div><h3>Strong Academics</h3><p>Structured classroom learning with attention to concepts, regular practice and examination readiness.</p></div>
<div class="card reveal"><div class="icon">🔬</div><h3>Science & Practical Work</h3><p>Hands-on science learning using laboratory equipment, experiments, demonstrations and project-based activities.</p></div>
<div class="card reveal"><div class="icon">💻</div><h3>Computer Education</h3><p>Computer lab activities, digital literacy, coding and technology-focused learning for students.</p></div>
</div>
</div>
</section>
 
<section class="dark">
<div class="container">
<div class="section-head reveal"><div class="eyebrow" style="color:var(--gold)">School at a Glance</div><h2>Learning, Participation & Development</h2><p>Key areas visible across the school's learning environment.</p></div>
<div class="stats">
<div class="stat"><strong>01</strong><span>Science & Practical Learning</span></div>
<div class="stat"><strong>02</strong><span>Computer & Digital Learning</span></div>
<div class="stat"><strong>03</strong><span>Sports & Co-curricular Activities</span></div>
<div class="stat"><strong>04</strong><span>School Events & Student Participation</span></div>
</div>
</div>
</section>
 
<section id="facilities" style="background:#f7fafc">
<div class="container">
<div class="section-head reveal"><div class="eyebrow">Campus & Facilities</div><h2>Spaces Designed for Learning</h2><p>Explore the learning and activity spaces visible in our school photographs.</p></div>
<div class="facility-grid">
<div class="facility reveal"><div class="icon">🧪</div><div><h3>Science Laboratory</h3><p>Practical demonstrations and experiment-based science learning.</p></div></div>
<div class="facility reveal"><div class="icon">🖥️</div><div><h3>Computer Laboratory</h3><p>Hands-on computer use, digital learning and coding practice.</p></div></div>
<div class="facility reveal"><div class="icon">📖</div><div><h3>Classrooms</h3><p>Dedicated spaces for classroom teaching and student interaction.</p></div></div>
<div class="facility reveal"><div class="icon">🏃</div><div><h3>Sports & Outdoor Space</h3><p>Outdoor participation that encourages fitness and teamwork.</p></div></div>
<div class="facility reveal"><div class="icon">🎨</div><div><h3>Creative Activities</h3><p>Art, cultural programmes, exhibitions and student projects.</p></div></div>
<div class="facility reveal"><div class="icon">🚌</div><div><h3>School Campus</h3><p>A campus environment supporting academic and co-curricular activities.</p></div></div>
</div>
</div>
</section>
 
<section id="activities">
<div class="container">
<div class="section-head reveal"><div class="eyebrow">Student Life</div><h2>Activities That Build Confidence</h2><p>Students get opportunities to participate, create, collaborate and present their learning.</p></div>
<div class="cards">
<div class="card reveal"><div class="icon">👩💻</div><h3>Coding Club</h3><p>Technology activities, computer practice, coding concepts and digital creativity.</p></div>
<div class="card reveal"><div class="icon">🎤</div><h3>School Events</h3><p>Assemblies, celebrations, exhibitions and events that bring the school community together.</p></div>
<div class="card reveal"><div class="icon">🏅</div><h3>Sports & Teamwork</h3><p>Physical activities and sports encourage discipline, teamwork and a healthy competitive spirit.</p></div>
</div>
</div>
</section>
 
<section class="intro" id="notices">
<div class="container">
<div class="section-head reveal"><div class="eyebrow">School Information</div><h2>Notices & Quick Information</h2><p>Important information can be updated here by editing one section of the website.</p></div>
<div class="notice-wrap">
<div class="notice-box reveal"><h3>📢 Latest Notices</h3><ul>
<li><time>NOTICE</time>Admission enquiries for the new academic session can be made through the school office.</li>
<li><time>ACADEMICS</time>Students should follow the academic calendar and instructions issued by the school.</li>
<li><time>ACTIVITIES</time>School activities, exhibitions and competitions are conducted throughout the academic year.</li>
</ul></div>
<div class="notice-box reveal"><h3>📅 Quick Links</h3><ul>
<li><a href="#academics">→ Academic Programmes</a></li>
<li><a href="#facilities">→ Campus & Facilities</a></li>
<li><a href="#activities">→ Student Activities</a></li>
<li><a href="#gallery">→ Photo Gallery</a></li>
<li><a href="#contact">→ Contact / Enquiry</a></li>
</ul></div>
</div>
</div>
</section>
 
<section id="gallery">
<div class="container">
<div class="section-head reveal"><div class="eyebrow">Gallery</div><h2>Life at T.I.T. Senior Secondary School</h2><p>Click any photo to view it larger.</p></div>
<div class="gallery">
<figure class="reveal"><img src="images/school-photo-01.jpg" alt="School campus and event"><figcaption>School Event</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-02.jpg" alt="Students and teachers at school event"><figcaption>Student Participation</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-03.jpg" alt="Science practical classroom"><figcaption>Science Learning</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-04.jpg" alt="Computer laboratory"><figcaption>Computer Lab</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-05.jpg" alt="Computer lab activity"><figcaption>Digital Learning</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-06.jpg" alt="School campus outdoor area"><figcaption>Campus</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-07.jpg" alt="Classroom learning"><figcaption>Classroom</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-08.jpg" alt="Science practical equipment"><figcaption>Practical Equipment</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-09.jpg" alt="Electronics and technology resources"><figcaption>Technology Resources</figcaption></figure>
<figure class="reveal"><img src="images/school-photo-10.jpg" alt="Students in classroom"><figcaption>Classroom Activity</figcaption></figure>
</div>
</div>
</section>
 
<section class="cta" id="admission">
<div class="container reveal"><h2>Interested in T.I.T. Senior Secondary School?</h2><p>For admission-related information, contact the school office or send an enquiry.</p><a class="btn btn-gold" href="#contact">Send an Enquiry →</a></div>
</section>
 
<section id="contact">
<div class="container">
<div class="section-head reveal"><div class="eyebrow">Contact</div><h2>Get in Touch</h2><p>Use the enquiry form for admission or general school-related questions.</p></div>
<div class="contact-grid">
<div class="contact-info reveal">
<h3>T.I.T. Senior Secondary School</h3>
<div class="contact-item"><b>Location</b>Bhiwani, Haryana, India</div>
<div class="contact-item"><b>Phone</b>+91 80595 99532</div>
<div class="contact-item"><b>Email</b>riki66277@gmail.com</div>
<div class="contact-item"><b>School</b>Senior Secondary School</div>
</div>
<form id="enquiryForm" class="reveal">
<div class="form-grid">
<div><label for="name">Parent / Student Name *</label><input id="name" required autocomplete="name"></div>
<div><label for="phone">Phone Number *</label><input id="phone" required inputmode="tel" pattern="[0-9+ ()-]{8,}" autocomplete="tel"></div>
<div><label for="email">Email</label><input id="email" type="email" autocomplete="email"></div>
<div><label for="class">Class</label><select id="class"><option>Not specified</option><option>Nursery / Primary</option><option>Middle School</option><option>Class 9</option><option>Class 10</option><option>Class 11</option><option>Class 12</option></select></div>
<div class="full"><label for="message">Message *</label><textarea id="message" required placeholder="Write your enquiry..."></textarea></div>
<div class="full"><button class="btn btn-blue" type="submit">Save Enquiry</button><div class="form-note">This static GitHub Pages version stores submitted enquiries in this browser only. No data is sent to a server.</div></div>
</div>
</form>
</div>
</div>
</section>
</main>
 
<footer>
<div class="container footer-grid">
<div><h3>T.I.T. Senior Secondary School</h3><p>Education, practical learning, technology, sports and student development in Bhiwani, Haryana.</p></div>
<div><h3>Explore</h3><ul><li><a href="#about">About</a></li><li><a href="#academics">Academics</a></li><li><a href="#facilities">Facilities</a></li><li><a href="#activities">Activities</a></li></ul></div>
<div><h3>Gallery</h3><ul><li><a href="#gallery">School Events</a></li><li><a href="#gallery">Science Lab</a></li><li><a href="#gallery">Computer Lab</a></li><li><a href="#gallery">Classrooms</a></li></ul></div>
<div><h3>Contact</h3><ul><li>Bhiwani, Haryana</li><li>+91 80595 99532</li><li>riki66277@gmail.com</li></ul></div>
</div>
<div class="container footer-bottom">© <span id="year"></span> T.I.T. Senior Secondary School, Bhiwani. All rights reserved.</div>
</footer>
 
<div class="lightbox" id="lightbox" role="dialog" aria-modal="true"><button class="lb-close" id="lbClose" aria-label="Close">×</button><img id="lbImage" alt=""><div class="lb-caption" id="lbCaption"></div></div>
<div class="toast" id="toast"></div>
<button class="to-top" id="toTop" aria-label="Back to top">↑</button>
 
<script>
const $=s=>document.querySelector(s), $$=s=>document.querySelectorAll(s);
$("#year").textContent=new Date().getFullYear();
 
$("#menuBtn").addEventListener("click",()=>$("#nav").classList.toggle("open"));
$$("nav a").forEach(a=>a.addEventListener("click",()=>$("#nav").classList.remove("open")));
 
const lightbox=$("#lightbox"), lbImage=$("#lbImage"), lbCaption=$("#lbCaption");
$$(".gallery figure").forEach(fig=>fig.addEventListener("click",()=>{
  const img=fig.querySelector("img"); lbImage.src=img.src; lbImage.alt=img.alt; lbCaption.textContent=fig.querySelector("figcaption").textContent; lightbox.classList.add("open");
}));
function closeLightbox(){lightbox.classList.remove("open");lbImage.src=""}
$("#lbClose").addEventListener("click",closeLightbox);
lightbox.addEventListener("click",e=>{if(e.target===lightbox)closeLightbox()});
document.addEventListener("keydown",e=>{if(e.key==="Escape")closeLightbox()});
 
$("#enquiryForm").addEventListener("submit",e=>{
  e.preventDefault();
  const item={
    name:$("#name").value.trim(),
    phone:$("#phone").value.trim(),
    email:$("#email").value.trim(),
    className:$("#class").value,
    message:$("#message").value.trim(),
    time:new Date().toLocaleString()
  };
  const list=JSON.parse(localStorage.getItem("titSchoolEnquiries")||"[]");
  list.push(item); localStorage.setItem("titSchoolEnquiries",JSON.stringify(list));
  e.target.reset();
  showToast("Enquiry saved successfully on this device.");
});
function showToast(msg){const t=$("#toast");t.textContent=msg;t.style.display="block";clearTimeout(window.toastTimer);window.toastTimer=setTimeout(()=>t.style.display="none",3500)}
 
const observer=new IntersectionObserver(entries=>entries.forEach(x=>{if(x.isIntersecting)x.target.classList.add("show")}),{threshold:.08});
$$(".reveal").forEach(x=>observer.observe(x));
 
window.addEventListener("scroll",()=>{$("#toTop").style.display=scrollY>500?"block":"none"});
$("#toTop").addEventListener("click",()=>scrollTo({top:0,behavior:"smooth"}));
</script>
</body>
</html>
