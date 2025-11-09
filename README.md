index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Shibin KS – Full Portfolio</title>

  <!-- Font Awesome -->
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css"
  />

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
      color: #333;
      background: #f4f4f4;
      overflow-x: hidden;
    }
    a {
      text-decoration: none;
      color: inherit;
    }
    img {
      max-width: 100%;
      display: block;
      border-radius: 8px;
    }
    .container {
      width: 90%;
      max-width: 1200px;
      margin: 0 auto;
    }

    /* Header / Nav */
    header {
      background: #222;
      color: #fff;
      padding: 20px 0;
    }
    .nav-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .nav-logo {
      font-size: 1.5rem;
      font-weight: 700;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 25px;
    }
    nav ul li a {
      color: #fff;
      font-weight: 500;
      transition: color 0.3s;
    }
    nav ul li a:hover {
      color: #00c6ff;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(to right, #007bff, #00c6ff);
      color: #fff;
      padding: 80px 20px;
      text-align: center;
    }
    .hero-content h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }
    .hero-content h2 {
      font-size: 1.5rem;
      margin-bottom: 20px;
    }
    .contact-info p {
      margin: 5px 0;
    }

    /* About Section */
    section {
      padding: 60px 0;
    }
    #about p {
      margin-bottom: 15px;
      text-align: justify;
    }

    /* Skills */
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
      color: #222;
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

    /* Experience */
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
      font-size: 1rem;
      padding: 8px;
      border-radius: 50%;
      width: 35px;
      height: 35px;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .timeline-content {
      background: #f9f9f9;
      padding: 15px;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.05);
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

    /* Projects */
    .works-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
      margin-top: 30px;
    }
    .work-content {
      margin-top: 10px;
    }

    /* Testimonials */
    .testimonials-flex {
      display: flex;
      flex-wrap: wrap;
      gap: 30px;
      justify-content: center;
      margin-top: 30px;
    }
    .testimonial-box {
      background: #f9f9f9;
      padding: 20px;
      border-radius: 8px;
      max-width: 350px;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.05);
      text-align: center;
    }

    /* Contact */
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
    .form-group input,
    .form-group textarea {
      flex: 1 1 100%;
      padding: 15px;
      font-size: 1rem;
      border: 2px solid #000;
      border-radius: 5px;
      background: #fff;
    }
    button[type='submit'] {
      padding: 15px 30px;
      font-size: 1.1rem;
      background-color: #000;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      align-self: center;
      transition: background-color 0.3s;
    }
    button[type='submit']:hover {
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

    /* Responsive */
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
      .hero-content h1 {
        font-size: 2.2rem;
      }
      .hero-content h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>

<body>
  <!-- Header -->
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

  <!-- Hero -->
  <section class="hero">
    <div class="hero-content container">
      <h1>Shibin KS</h1>
      <h2>Web Developer & Cyber security researcher  </h2>
      <div class="contact-info">
        <p><a href="mailto:cybernova171717@gmail.com">cybernova171717@gmail.com</a></p>
        <p>Phone: +91 8138030292  | Location: Ernakulam, Kerala</p>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="container">
    <h2 style="text-align:center;">About Me</h2>
    <p>
      > I’m an Ethical Hacker and Web Developer passionate about building secure, modern digital solutions. I specialize in penetration testing, vulnerability assessment, and full-stack web development, ensuring every project is protected from the ground up. My mission is to combine creativity with cybersecurity — crafting websites that look great and stay safe.
    </p>
    <p>
      I enjoy solving complex problems, optimizing performance, and turning ideas into functional digital products.
    </p>
  </section>

  <!-- Skills -->
  <section id="skills" class="container">
    <h2 style="text-align:center;">My Skills</h2>
    <div class="skills-bars">
      <div class="skill">
        <div class="skill-title">network sacnning (Nmap,wireshark,linux system,burpsuite,metaspoilt,Hydera</div>
        <div class="skill-bar"><div class="skill-fill" style="width:95%"></div></div>
      </div>
      <div class="skill">
        <div class="skill-title">CSS3 (Flexbox, Grid, Animations)</div>
        <div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div>
      </div>
      <div class="skill">
        <div class="skill-title">JavaScript & DOM Manipulation</div>
        <div class="skill-bar"><div class="skill-fill" style="width:85%"></div></div>
      </div>
      <div class="skill">
        <div class="skill-title">UI/UX Design (Figma, Prototyping)</div>
        <div class="skill-bar"><div class="skill-fill" style="width:80%"></div></div>
      </div>
    </div>
  </section>

  <!-- Experience -->
  <section id="experience" class="container">
    <h2 style="text-align:center;">Experience</h2>
    <div class="timeline">
      <div class="timeline-item">
        <div class="timeline-icon"><i class="fa-solid fa-briefcase"></i></div>
        <div class="timeline-content">
          <h3>Intern – XYZ Solutions</h3>
          <span> (3 Months)</span>
          <p>Cybersecurity Researcher with 3 months of practical experience exploring ethical hacking, penetration testing, and web application security. I've worked with tools like Burp Suite, Nmap, Wireshark, and Metasploit to identify and mitigate vulnerabilities. Alongside my interest in cybersecurity, I'm also learning MERN Stack Development to build and secure modern web applications from both the developer and defender perspectives.</p>
        </div>
      </div>
      <div class="timeline-item">
        <div class="timeline-icon"><i class="fa-solid fa-code"></i></div>
        <div class="timeline-content">
          <h3>Freelancer – Web Projects</h3>
          <span>2025 – Present</span>
          <p>Developed and deployed websites for local businesses with SEO and mobile optimization.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects -->
  <section id="portfolio" class="container">
    <h2 style="text-align:center;">Projects</h2>
    <div class="works-grid">
      <div class="work-item">
        <img src="img1.jpg" alt="Startup Website Project" />
        <div class="work-content">
          <h3>Startup Website</h3>
          <p>Landing page for a startup brand with conversion-focused design.</p>
        </div>
      </div>
      <div class="work-item">
        <img src="img2.jpg" alt="App UI Design Project" />
        <div class="work-content">
          <h3>App UI Design</h3>
          <p>Modern mobile UI designed in Figma and built with HTML/CSS prototype.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonials -->
  <section id="testimonials" class="container">
    <h2 style="text-align:center;">What Clients Say</h2>
    <div class="testimonials-flex">
      <div class="testimonial-box">
        <p>“Shibin delivered our website ahead of schedule and it looks fantastic.”</p>
        <h4>John Doe – CEO, Startup Inc.</h4>
      </div>
      <div class="testimonial-box">
        <p>“Working with Shibin was smooth: great communication and top-notch results.”</p>
        <h4>Jane Smith – Marketing Lead, BrandCo</h4>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <div class="container">
      <h2 style="text-align:center;">Contact Me</h2>
      <p>Let's build something great together. Drop me a message!</p>
      <form class="contact-form" action="#" method="POST">
        <div class="form-group">
          <input type="text" name="name" placeholder="Your Name" required />
        </div>
        <div class="form-group">
          <input type="email" name="email" placeholder="Your Email" required />
        </div>
        <div class="form-group">
          <input type="text" name="subject" placeholder="Subject" required />
        </div>
        <div class="form-group">
          <textarea name="message" rows="6" placeholder="Your Message" required></textarea>
        </div>
        <button type="submit">Send Message</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <p>&copy; 2025. All rights reserved.</p>
    </div>
  </footer>
</body>
</html>


