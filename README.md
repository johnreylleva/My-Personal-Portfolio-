# My-Personal-Portfolio-<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>John Rey Lleva | Aspiring Game Developer</title>
  <!-- Google Fonts + Font Awesome -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(145deg, #f0f4fc 0%, #e8eff9 100%);
      color: #1a2c3e;
      line-height: 1.5;
      padding: 2rem 1.5rem;
    }

    /* main container – clean card */
    .container {
      max-width: 1050px;
      margin: 0 auto;
      background: #ffffff;
      border-radius: 2rem;
      box-shadow: 0 25px 45px -12px rgba(0, 0, 0, 0.15);
      overflow: hidden;
      transition: all 0.2s ease;
    }

    /* inner spacing */
    .inner-content {
      padding: 2rem 2.2rem 1.8rem 2.2rem;
    }

    /* ========== PROFILE SECTION ========== */
    .profile-section {
      margin-bottom: 2rem;
      border-bottom: 2px solid #eef2f8;
      padding-bottom: 1.6rem;
    }

    .profile-inner {
      display: flex;
      align-items: center;
      gap: 2rem;
      flex-wrap: wrap;
      justify-content: center;
    }

    /* 2x2 picture wrapper – formal, crisp */
    .profile-img-wrapper {
      flex-shrink: 0;
      width: 150px;
      height: 150px;
      background: #f0f5fc;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 12px 22px -8px rgba(0, 0, 0, 0.1);
      border: 3px solid white;
      outline: 1px solid #d4e0ec;
      transition: transform 0.2s;
    }

    .profile-img-wrapper:hover {
      transform: scale(1.02);
    }

    .profile-img {
      width: 150px;
      height: 150px;
      object-fit: cover;
      border-radius: 50%;
      display: block;
    }

    .profile-info {
      text-align: left;
    }

    .full-name {
      font-size: 2.1rem;
      font-weight: 800;
      letter-spacing: -0.02em;
      background: linear-gradient(135deg, #1a4970, #2c6e9e);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      margin-bottom: 0.5rem;
    }

    .title-tag {
      font-size: 1.2rem;
      font-weight: 600;
      color: #2c6e9e;
      background: #eef3fc;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.4rem 1.2rem;
      border-radius: 60px;
      backdrop-filter: blur(2px);
    }

    /* section headings – modern blue accent */
    .section-title {
      font-size: 1.65rem;
      font-weight: 700;
      margin: 2rem 0 1rem 0;
      color: #1a4c6e;
      display: flex;
      align-items: center;
      gap: 12px;
      border-left: 5px solid #2c7ab1;
      padding-left: 1rem;
    }

    .section-title:first-of-type {
      margin-top: 0;
    }

    .section-title i {
      color: #2c7ab1;
      font-size: 1.5rem;
    }

    /* about me paragraph – soft blueish background */
    .about-text {
      background: #f6faff;
      padding: 1.3rem 1.8rem;
      border-radius: 1.5rem;
      font-size: 1rem;
      line-height: 1.65;
      color: #1f3e54;
      border: 1px solid #e6edf8;
      transition: all 0.2s;
    }

    /* Personal info – elegant table style */
    .personal-card {
      background: #f6faff;
      border-radius: 1.5rem;
      padding: 0.2rem;
      border: 1px solid #e6edf8;
      overflow-x: auto;
    }

    .info-table {
      width: 100%;
      border-collapse: collapse;
    }

    .info-table tr {
      border-bottom: 1px solid #e2ebf5;
    }

    .info-table tr:last-child {
      border-bottom: none;
    }

    .info-table td {
      padding: 1rem 1.3rem;
      font-size: 0.98rem;
    }

    .info-table td:first-child {
      font-weight: 700;
      color: #1f6392;
      width: 160px;
      letter-spacing: -0.2px;
    }

    .info-table td:last-child {
      color: #1e3a4d;
      font-weight: 500;
    }

    /* skills – clean list with subtle blue */
    .skills-container {
      background: #f6faff;
      border-radius: 1.5rem;
      padding: 1.3rem 1.8rem;
      border: 1px solid #e6edf8;
    }

    .skill-item {
      display: flex;
      flex-wrap: wrap;
      align-items: baseline;
      padding: 0.8rem 0;
      border-bottom: 1px solid #e4edf7;
    }

    .skill-item:last-child {
      border-bottom: none;
    }

    .skill-name {
      font-weight: 700;
      color: #1e4a6e;
      width: 130px;
      flex-shrink: 0;
      font-size: 1rem;
    }

    .skill-level {
      color: #2c607e;
      font-weight: 500;
    }

    /* inspiration block – blue border left, with tiny emerald accent */
    .inspiration-block {
      background: #f0f7fe;
      padding: 1.6rem 2rem;
      border-radius: 1.5rem;
      margin-top: 0.3rem;
      border-left: 6px solid #2c7ab1;
      font-size: 1rem;
      line-height: 1.68;
      color: #1c405b;
      transition: all 0.2s;
      box-shadow: 0 2px 5px rgba(0,0,0,0.02);
    }

    /* footer */
    .footer-note {
      text-align: center;
      margin-top: 2.5rem;
      padding-top: 1.3rem;
      border-top: 1px solid #e2edf5;
      font-size: 0.85rem;
      color: #6f8eaa;
      font-weight: 500;
    }

    /* responsive */
    @media (max-width: 720px) {
      .inner-content {
        padding: 1.5rem;
      }
      .profile-inner {
        flex-direction: column;
        text-align: center;
      }
      .profile-info {
        text-align: center;
      }
      .full-name {
        font-size: 1.7rem;
      }
      .info-table td {
        padding: 0.8rem 1rem;
        display: table-cell;
      }
      .skill-name {
        width: 110px;
      }
      .section-title {
        font-size: 1.45rem;
      }
    }

    @media (max-width: 550px) {
      .info-table, .info-table tbody, .info-table tr, .info-table td {
        display: block;
      }
      .info-table tr {
        display: block;
        margin-bottom: 0.6rem;
        border-bottom: 1px solid #e0e8f0;
      }
      .info-table td {
        display: flex;
        justify-content: space-between;
        align-items: center;
        border-bottom: none;
        padding: 0.7rem 0.8rem;
      }
      .info-table td:first-child {
        width: auto;
      }
      .info-table td:last-child {
        text-align: right;
      }
      .skill-item {
        flex-direction: column;
        gap: 0.2rem;
      }
      .skill-name {
        width: auto;
      }
    }

    /* hover effect on cards */
    .about-text:hover, .personal-card:hover, .skills-container:hover, .inspiration-block:hover {
      background: #ffffff;
      border-color: #cfdff0;
      transition: 0.2s;
    }
  </style>
</head>
<body>
<div class="container">
  <div class="inner-content">
    <!-- PROFILE SECTION: Name + Title + 2x2 picture -->
    <header class="profile-section">
      <div class="profile-inner">
        <!-- 2x2 picture: replace 'profile-picture.jpg' with your actual 2x2 image file -->
        <div class="profile-img-wrapper">
          <img src="[profile-picture.jpg](https://github.com/johnreylleva/My-Personal-Portfolio-/blob/2f174e027b00b69b3361034550f1dc85b2e42e3b/1776307235967.png)" alt="2x2 formal photo of John Rey Villanueva Lleva" class="profile-img">
        </div>
        <div class="profile-info">
          <h1 class="full-name">John Rey Villanueva Lleva</h1>
          <p class="title-tag"><i class="fas fa-gamepad"></i> ASPIRING GAME DEVELOPER</p>
        </div>
      </div>
    </header>

    <!-- ABOUT ME section: revised, personal and professional -->
    <section>
      <h2 class="section-title"><i class="fas fa-user-astronaut"></i> About Me</h2>
      <div class="about-text">
        I am a dedicated first-year BSIT student at <strong>Our Lady of the Sacred Heart College of Guimba</strong>, deeply passionate about technology and how it shapes the future. 
        My curiosity drives me to explore the intersection of logic, creativity, and user experience — from coding interactive applications to designing seamless digital interfaces. 
        I believe that software should not only function flawlessly but also inspire and empower its users. As I progress in my IT journey, I strive to master both front-end 
        craftsmanship and backend problem-solving, turning innovative ideas into meaningful, real-world solutions.
      </div>
    </section>

    <!-- PERSONAL DETAILS section (updated: Guiset, email, age, name) -->
    <section>
      <h2 class="section-title"><i class="fas fa-id-card"></i> Personal Information</h2>
      <div class="personal-card">
        <table class="info-table">
          <tr>
            <td><i class="fas fa-user-circle" style="margin-right: 8px; color:#2c7ab1;"></i> FULL NAME</td>
            <td>John Rey Villanueva Lleva</td>
          </tr>
          <tr>
            <td><i class="fas fa-calendar-alt" style="margin-right: 8px; color:#2c7ab1;"></i> AGE</td>
            <td>18 Years Old</td>
          </tr>
          <tr>
            <td><i class="fas fa-envelope" style="margin-right: 8px; color:#2c7ab1;"></i> EMAIL ADDRESS</td>
            <td>johnreylleva22@gmail.com</td>
          </tr>
          <tr>
            <td><i class="fas fa-map-marker-alt" style="margin-right: 8px; color:#2c7ab1;"></i> ADDRESS</td>
            <td>Guiset, Guimba, Nueva Ecija</td>
          </tr>
        </table>
      </div>
    </section>

    <!-- SKILLS & PROGRAMMING LANGUAGES (keeping the original structure) -->
    <section>
      <h2 class="section-title"><i class="fas fa-laptop-code"></i> Skills & Programming Languages</h2>
      <div class="skills-container">
        <div class="skill-item">
          <span class="skill-name"><i class="fab fa-java" style="margin-right: 8px;"></i> Java:</span>
          <span class="skill-level">Beginner (Developing system logic and UI)</span>
        </div>
        <div class="skill-item">
          <span class="skill-name"><i class="fab fa-python" style="margin-right: 8px;"></i> Python:</span>
          <span class="skill-level">Beginner</span>
        </div>
        <div class="skill-item">
          <span class="skill-name"><i class="fab fa-html5" style="margin-right: 8px;"></i> HTML & CSS:</span>
          <span class="skill-level">Mid (Intermediate proficiency, responsive design)</span>
        </div>
      </div>
    </section>

    <!-- INSPIRATION section: updated to Pokémon Emerald and its creator -->
    <section>
      <h2 class="section-title"><i class="fas fa-leaf" style="color:#2c7ab1;"></i> Inspiration</h2>
      <div class="inspiration-block">
        <p>My journey in game development is deeply inspired by <strong>Pokémon Emerald Green</strong> — a game that shaped my childhood and ignited my curiosity for interactive storytelling. 
        The creator behind the Pokémon franchise, <strong>Satoshi Tajiri</strong>, envisioned a world where creatures and humans connect through adventure and friendship. 
        Seeing how a simple idea evolved into a global phenomenon taught me that great games are born from passion and attention to detail. 
        Tajiri’s dedication to building immersive worlds motivates me to not only write functional code but to craft experiences that evoke wonder and joy. 
        As an aspiring game developer, I aim to bring the same level of heart, depth, and creativity into every project I build — turning pixels into memories.</p>
      </div>
    </section>

    <!-- FOOTER with updated name -->
    <footer class="footer-note">
      <p>© 2026 John Rey Villanueva Lleva | HCI101 Final Project</p>
    </footer>
  </div>
</div>
</body>
</html>
