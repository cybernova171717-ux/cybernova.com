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
      padding: 15px

