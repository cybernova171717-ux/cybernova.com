<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
<title>Shibin KS – Full Portfolio</title>
<style>
/* Reset & base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  color: #723e3e;
  background: #662121;
  overflow-x: hidden;
}
a {
  text-decoration: none;
}
img {
  max-width: 100%;
  display: block;
}
.container {
  width: 90%;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: -20%;
}
/* Header / Nav */
header {
  background: #222;
  color: #fff;
}
text-align: center;
}
#contact p {
  font-size: 1.1rem;
  margin-bottom: 30px;
  color: #555;
  text-align: center;
}
.contact-form {
  display: flex;
  flex-direction: column;
  gap: 20px;
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
}
.form-group {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}
.form-group input,
.form-group textarea {
  flex: 1 1 100%;
  padding: 15px;
  font-size: 1rem;
  border: 2px solid #000;
  border-radius: 5px;
  background: #fff;
}
button[type="submit"] {
  padding: 15px 30px;
  font-size: 1.1rem;
  background-color: #000;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  align-self: center;
}
button[type="submit"]:hover {
  background-color: #444;
}
/* Footer */
footer {
  background: #222;
  color: #ccc;
  text-align: center;
  padding: 30px 0;
  margin-top: 40px;
}
footer p {
  margin: 0;
}
/* Responsive adjustments */
@media (max-width: 768px) {
  .nav-container {
    flex-direction: column;
    align-items: flex-start;
  }
  nav ul {
    flex-direction: column;
    gap: 10px;
    margin-top: 15px;
  }
  .skills-flex, .experience-flex, .works-grid, .testimonials-flex {
    flex-direction: column;
  }
  .skill-box, .exp-box, .work-item, .testimonial-box {
    flex: 1 1 100%;
  }
  .hero-content h1 {
    font-size: 2.5rem;
  }
  .hero-content h2 {
    font-size: 1.2rem;
  }
}
.skills-bars {
  margin-top: 30px;
  display: flex;
  flex-direction: column;
  gap: 25px;
}
.skill {
  width: 100%;
}
.skill-title {
  font-size: 1.1rem;
  margin-bottom: 8px;
  color: #333;
  font-weight: 600;
}
.skill-bar {
  width: 100%;
  background-color: #e6e6e6;
  height: 12px;
  border-radius: 6px;
  overflow: hidden;
}
.skill-fill {
  height: 100%;
  background: linear-gradient(to right, #007bff, #00c6ff);
  border-radius: 6px;
  transition: width 0.8s ease-in-out;
}
.timeline {
  position: relative;
  margin-top: 40px;
  padding-left: 30px;
  border-left: 3px solid #007bff;
}
.timeline-item {
  position: relative;
  margin-bottom: 40px;
}
.timeline-icon {
  position: absolute;
  left: -25px;
  top: 10px;
  background-color: #007bff;
  color: #fff;
  font-size: 1.2rem;
  padding: 10px;
  padding-top: 15px;
  border-radius: 50%;
  width: 35px;
  height: 35px;
  text-align: center;
  line-height: 15px;
  padding-bottom: 6px;
}
.timeline-content {
  background: #f9f9f9;
  padding: 10px;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
}
.timeline-content h3 {
  margin-bottom: 5px;
  color: #222;
}
.timeline-content span {
  font-size: 0.9rem;
  color: #777;
  display: block;
  margin-bottom: 10px;
}
.timeline-content p {
  font-size: 1rem;
  color: #555;
}
</style>
</head>
<body>
<!-- Header / Navigation -->
<header>
  <div class="container nav-container">
    <div class="nav-logo">Freelancer</div>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#portfolio">Projects</a></li>
        <li><a href="#testimonials">Testimonials</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </div>
</header>

<!-- Hero / Intro -->
<section class="hero">
  <div class="hero-content container">
    <h1>Shibin KS</h1>
    <h2>Web Developer, Ethical Hacker & UI/UX Designer</h2>
    <div class="contact-info">
      <p><a href="mailto:shibinks@gmail.com">shibinks@gmail.com</a></p>
      <p>Phone: | Location: Ernakulam, Kerala</p>
    </div>
  </div>
</section>

<!-- About Section -->
<section id="about" class="container">
  <h2 style="text-align: center;">About Me</h2>
  <p>I’m a passionate MERN Stack

