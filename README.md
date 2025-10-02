<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Rahma Maaroufi | Portfolio</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;600;800&display=swap');

    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; }

    body {
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      color: #fff;
      scroll-behavior: smooth;
      line-height: 1.6;
    }

    header {
      display: flex; justify-content: space-between; align-items: center;
      padding: 20px 60px; background: rgba(0, 0, 0, 0.3);
      position: fixed; width: 100%; top: 0; z-index: 1000;
      backdrop-filter: blur(10px);
    }
    header h1 { font-size: 24px; font-weight: 800; }
    nav a { margin: 0 15px; text-decoration: none; color: #fff; font-weight: 600; transition: 0.3s; }
    nav a:hover { color: #ff4f81; }

    section { padding: 100px 60px; }

    .hero { display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; min-height: 100vh; padding-top:120px; }
    .hero-text { max-width: 600px; }
    .hero-text h2 { font-size: 22px; margin-bottom: 10px; font-weight: 500; }
    .hero-text h1 {
      font-size: 48px; font-weight: 800;
      background: linear-gradient(90deg, #ff758c, #ff7eb3);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent;
    }
    .hero-text p { margin: 20px 0; font-size: 18px; }

    .buttons a {
      text-decoration: none; padding: 12px 25px; border-radius: 25px;
      background: #fff; color: #ff4f81; font-weight: 600; margin-right: 15px; transition: 0.3s;
    }
    .buttons a:hover { 
      transform: translateY(-3px); 
      box-shadow: 0 8px 15px rgba(0,0,0,0.2);
      background: #ff4f81; 
      color: #fff; 
    }

    .hero-img img {
      width: 300px; height: 300px; border-radius: 50%;
      border: 6px solid #fff; box-shadow: 0 0 30px rgba(255, 118, 157, 0.8);
    }

    h2.section-title {
      font-size: 36px; margin-bottom: 40px; font-weight: 800;
      text-align: center;
      background: linear-gradient(90deg, #ff758c, #ff7eb3);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent;
    }

    .skills-container, .projects-container, .certifications-container {
      display: flex; flex-wrap: wrap; justify-content: center; gap: 30px;
    }
    .skill-box, .project-box, .cert-box {
      background: rgba(255, 255, 255, 0.1);
      padding: 25px 30px; border-radius: 15px; min-width: 220px;
      text-align: center; transition: 0.3s;
      box-shadow: 0 4px 15px rgba(0,0,0,0.2);
    }
    .skill-box:hover, .project-box:hover, .cert-box:hover {
      transform: scale(1.05); background: rgba(255, 255, 255, 0.2);
    }

    /* CONTACT */
    #contact form { max-width: 600px; margin: auto; display: flex; flex-direction: column; gap: 15px; }
    #contact input, #contact textarea {
      padding: 15px; border-radius: 10px; border: none; outline: none; font-size: 16px;
    }
    #contact button {
      padding: 15px; border-radius: 10px; border: none;
      background: #fff; color: #ff4f81; font-weight: 600; cursor: pointer; transition: 0.3s;
      font-size: 16px;
    }
    #contact button:hover { background: #ff4f81; color: #fff; }

    /* ANIMATIONS */
    @keyframes fadeInUp {
      0% { opacity: 0; transform: translateY(20px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    .section-title, .skills-container .skill-box, 
    .projects-container .project-box, .certifications-container .cert-box {
      opacity: 0;
      animation: fadeInUp 1s ease forwards;
    }

    .skills-container .skill-box { animation-delay: 0.2s; }
    .skills-container .skill-box:nth-child(2) { animation-delay: 0.4s; }
    .skills-container .skill-box:nth-child(3) { animation-delay: 0.6s; }
    .skills-container .skill-box:nth-child(4) { animation-delay: 0.8s; }
    .skills-container .skill-box:nth-child(5) { animation-delay: 1s; }
    .skills-container .skill-box:nth-child(6) { animation-delay: 1.2s; }

    .projects-container .project-box { animation-delay: 0.3s; }
    .projects-container .project-box:nth-child(2) { animation-delay: 0.6s; }

    .certifications-container .cert-box { animation-delay: 0.3s; }
    .certifications-container .cert-box:nth-child(2) { animation-delay: 0.6s; }

    .hero-text h1, .hero-text h2, .hero-text p {
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 1s ease forwards;
    }

    .hero-text h2 { animation-delay: 0.2s; }
    .hero-text h1 { animation-delay: 0.5s; }
    .hero-text p { animation-delay: 0.8s; }

    /* Responsive */
    @media (max-width: 900px) {
      .hero { flex-direction: column-reverse; text-align: center; }
      .hero-text { max-width: 100%; }
      .hero-img img { margin-bottom: 30px; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Rahma Maaroufi</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#certifications">Certifications</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- HERO -->
  <section id="home" class="hero">
    <div class="hero-text">
      <h2>Hi, I am</h2>
      <h1>Rahma Maaroufi</h1>
      <p>
        I am a 3rd-year Computer Science student currently preparing my Final Year Project (PFE).  
        I am looking for a PFE internship opportunity where I can apply my knowledge, develop my skills,  
        and contribute to innovative projects.
      </p>
      <div class="buttons">
        <a href="#contact">Get In Touch</a>
        <a href="#">Download CV</a>
      </div>
    </div>
    <div class="hero-img">
      <img src="photorahma.jpg" alt="Rahma Maaroufi">
    </div>
  </section>

  <!-- SKILLS -->
  <section id="skills">
    <h2 class="section-title">My Skills</h2>
    <div class="skills-container">
      <div class="skill-box">Java, Python, C++, PHP, JavaScript</div>
      <div class="skill-box">Web Dev: HTML, CSS, React, Angular</div>
      <div class="skill-box">Databases: SQL, NoSQL, MongoDB</div>
      <div class="skill-box">AI/ML: TensorFlow, Scikit-learn</div>
      <div class="skill-box">Networking & Cybersecurity basics</div>
      <div class="skill-box">Git, GitHub, VS Code, Eclipse</div>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects">
    <h2 class="section-title">My Projects</h2>
    <div class="projects-container">
      <div class="project-box">
        <h3>Taskinus – Intelligent To-Do List</h3>
        <p>Full-stack app with PHP, HTML, CSS, JavaScript, SQL. Features: task scheduling, reminders, AI suggestions.</p>
      </div>
      <div class="project-box">
        <h3>2D Street Racing Game</h3>
        <p>Built with Unity (C#). Features: car movement, collisions, scoring system, animations & sound effects.</p>
      </div>
    </div>
  </section>

  <!-- CERTIFICATIONS -->
  <section id="certifications">
    <h2 class="section-title">Certifications</h2>
    <div class="certifications-container">
      <div class="cert-box">3+ International Certifications</div>
      <div class="cert-box">Courses in AI, Web Dev, Cybersecurity</div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2 class="section-title">Contact Me</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p style="text-align:center; margin-top:20px;">
      📍 Tunis, Tunisia | 📧 rahmamaaroufi487@gmail.com | 🔗 
      <a href="https://www.linkedin.com/in/maaroufi-rahma-30487b360/?locale=fr_FR" target="_blank" style="color:#fff;">LinkedIn</a> | 
      <a href="https://github.com/rahmamaaroufi/Rahma_Maaroufi.tn" target="_blank" style="color:#fff;">GitHub</a>
    </p>
  </section>
</body>
</html>
