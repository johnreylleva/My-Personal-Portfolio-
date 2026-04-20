# My-Personal-Portfolio-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Prince Alfie Solomon | Aspiring Game Developer</title>
  <!-- Google Fonts for clean typography -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
  <!-- Font Awesome 6 (free icons) for subtle accents -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    /* RESET & BASE */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: #f5f7fb;
      color: #1a2c3e;
      line-height: 1.5;
      padding: 2rem 1.5rem;
    }

    .container {
      max-width: 1000px;
      margin: 0 auto;
      background: #ffffff;
      border-radius: 28px;
      box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.08);
      overflow: hidden;
      padding: 2rem 2rem 1.5rem 2rem;
    }

    /* ========== PROFILE SECTION ========== */
    .profile-section {
      margin-bottom: 2.2rem;
      border-bottom: 2px solid #eef2f7;
      padding-bottom: 1.8rem;
    }

    .profile-inner {
      display: flex;
      align-items: center;
      gap: 2rem;
      flex-wrap: wrap;
      justify-content: center;
    }

    .profile-img-wrapper {
      flex-shrink: 0;
      width: 150px;
      height: 150px;
      border-radius: 50%;
      background: #eef2f7;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 8px 18px rgba(0, 0, 0, 0.05);
      border: 3px solid white;
      outline: 1px solid #e0e8f0;
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
      font-size: 2rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      color: #0a2b3e;
      margin-bottom: 0.4rem;
    }

    .title-tag {
      font-size: 1.2rem;
      font-weight: 500;
      color: #2c6e9e;
      background: #eef3fc;
      display: inline-block;
      padding: 0.3rem 1rem;
      border-radius: 40px;
    }

    /* Section headings */
    .section-title {
      font-size: 1.6rem;
      font-weight: 600;
      margin: 1.8rem 0 1rem 0;
      color: #1e4663;
      border-left: 5px solid #2c7ab1;
      padding-left: 1rem;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .section-title:first-of-type {
      margin-top: 0;
    }

    .section-title i {
      color: #2c7ab1;
      font-size: 1.5rem;
    }

    /* About me paragraph */
    .about-text {
      font-size: 1rem;
      color: #2c3f4f;
      line-height: 1.65;
      background: #f9fbfd;
      padding: 1.2rem 1.5rem;
      border-radius: 20px;
      margin-top: 0.2rem;
    }

    /* PERSONAL DETAILS — Table style (clean and aligned) */
    .personal-table-wrapper {
      background: #f9fbfd;
      border-radius: 20px;
      padding: 0.2rem;
      overflow-x: auto;
    }

    .personal-table {
      width: 100%;
      border-collapse: collapse;
      background: #f9fbfd;
      border-radius: 18px;
    }

    .personal-table td {
      padding: 1rem 1.2rem;
      border-bottom: 1px solid #e6edf4;
      font-size: 0.98rem;
    }

    .personal-table tr:last-child td {
      border-bottom: none;
    }

    .personal-table td:first-child {
      font-weight: 700;
      color: #1f6392;
      width: 150px;
      letter-spacing: -0.2px;
    }

    .personal-table td:last-child {
      color: #1e2f3c;
      font-weight: 500;
    }

    /* Skills section (list style with levels) */
    .skills-list {
      background: #f9fbfd;
      border-radius: 20px;
      padding: 1.2rem 1.8rem;
      list-style: none;
    }

    .skills-list li {
      padding: 0.7rem 0;
      border-bottom: 1px solid #e6edf4;
      display: flex;
      flex-wrap: wrap;
      align-items: baseline;
      font-size: 1rem;
    }

    .skills-list li:last-child {
      border-bottom: none;
    }

    .skill-name {
      font-weight: 700;
      color: #1e4663;
      width: 130px;
      flex-shrink: 0;
    }

    .skill-desc {
      color: #2c4e6e;
    }

    /* Inspiration section */
    .inspiration-card {
      background: #f0f6fe;
      padding: 1.5rem 2rem;
      border-radius: 20px;
      margin-top: 0.3rem;
      border-left: 4px solid #2c7ab1;
      font-size: 1rem;
      line-height: 1.65;
      color: #1c405b;
    }

    /* Footer */
    .portfolio-footer {
      text-align: center;
      margin-top: 2.5rem;
      padding-top: 1.2rem;
      border-top: 1px solid #e2edf5;
      font-size: 0.85rem;
      color: #6a8aaa;
    }

    /* Responsive adjustments */
    @media (max-width: 700px) {
      .container {
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
      .personal-table td:first-child {
        width: 120px;
      }
      .personal-table td {
        padding: 0.8rem 0.8rem;
        display: table-cell;
      }
      .skill-name {
        width: 110px;
      }
      .section-title {
        font-size: 1.4rem;
      }
    }

    @media (max-width: 550px) {
      .personal-table, .personal-table tbody, .personal-table tr, .personal-table td {
        display: block;
      }
      .personal-table tr {
        margin-bottom: 0.5rem;
        border-bottom: 1px solid #e0e8f0;
        display: block;
      }
      .personal-table td {
        display: flex;
        justify-content: space-between;
        align-items: center;
        border-bottom: none;
        padding: 0.6rem 0.8rem;
      }
      .personal-table td:first-child {
        width: auto;
        font-weight: 700;
      }
      .personal-table td:last-child {
        text-align: right;
      }
    }
  </style>
</head>
<body>
<div class="container">
  <!-- SECTION 1: PROFILE (Name, Title, 2x2 Picture) -->
  <header class="profile-section">
    <div class="profile-inner">
      <!-- 2x2 Picture: use your own file named "profile-picture.jpg" or change src -->
      <div class="profile-img-wrapper">
        <img src="profile-picture.jpg" alt="2x2 photo of Prince Alfie Solomon, aspiring game developer" class="profile-img">
      </div>
      <div class="profile-info">
        <h1 class="full-name">Prince Alfie Fernando Solomon</h1>
        <p class="title-tag"><i class="fas fa-gamepad"></i> Aspiring Game Developer</p>
      </div>
    </div>
  </header>

  <!-- SECTION 2: ABOUT ME (course, school, interest in technology) -->
  <section>
    <h2 class="section-title"><i class="fas fa-user-astronaut"></i> About Me</h2>
    <p class="about-text">
      I am a first-year BSIT student at <strong>Our Lady of the Sacred Heart College of Guimba</strong>, with a growing passion for technology and continuous learning. 
      I'm especially interested in how software is built and how it can improve everyday tasks, making systems more efficient and user-friendly. 
      I enjoy exploring how logic and design work together — whether it's coding, designing interfaces, or understanding how users interact with a system. 
      As I continue learning, I focus on improving my skills and turning ideas into practical and functional solutions.
    </p>
  </section>

  <!-- SECTION 3: PERSONAL DETAILS (table format, clean & aligned) -->
  <section>
    <h2 class="section-title"><i class="fas fa-id-card"></i> Personal Details</h2>
    <div class="personal-table-wrapper">
      <table class="personal-table">
        <tr>
          <td><i class="fas fa-user-circle" style="margin-right: 8px; color:#2c7ab1;"></i> FULL NAME</td>
          <td>Prince Alfie Fernando Solomon</td>
        </tr>
        <tr>
          <td><i class="fas fa-calendar-alt" style="margin-right: 8px; color:#2c7ab1;"></i> AGE</td>
          <td>21 Years Old</td>
        </tr>
        <tr>
          <td><i class="fas fa-envelope" style="margin-right: 8px; color:#2c7ab1;"></i> EMAIL ADDRESS</td>
          <td>palfiesolomon@gmail.com</td>
        </tr>
        <tr>
          <td><i class="fas fa-map-marker-alt" style="margin-right: 8px; color:#2c7ab1;"></i> ADDRESS</td>
          <td>Bacayao Guimba, Nueva Ecija</td>
        </tr>
      </table>
    </div>
  </section>

  <!-- SECTION 4: SKILLS / PROGRAMMING LANGUAGES (with levels) -->
  <section>
    <h2 class="section-title"><i class="fas fa-laptop-code"></i> Skills & Programming Languages</h2>
    <ul class="skills-list">
      <li>
        <span class="skill-name">Java:</span>
        <span class="skill-desc">Beginner (Developing system logic and UI)</span>
      </li>
      <li>
        <span class="skill-name">Python:</span>
        <span class="skill-desc">Beginner</span>
      </li>
      <li>
        <span class="skill-name">HTML & CSS:</span>
        <span class="skill-desc">Mid (Intermediate proficiency)</span>
      </li>
    </ul>
  </section>

  <!-- SECTION 5: INSPIRATION AS A PROGRAMMER -->
  <section>
    <h2 class="section-title"><i class="fas fa-lightbulb"></i> Inspiration</h2>
    <div class="inspiration-card">
      <p>My journey in IT is inspired by the story of <strong>Eric Barone</strong>, the creator of Stardew Valley. 
      Seeing how one person could build an entire world — handling the code, the art, and the music — completely changed how I view what's possible in software development. 
      I'm driven by that same mindset. As an aspiring game developer, I don't just want to write code; I want to understand how logic and creativity work together to create meaningful experiences. 
      Barone's dedication motivates me to keep improving my skills and reminds me that with persistence, even a single developer can create something that connects with millions.</p>
    </div>
  </section>

  <!-- FOOTER with copyright and HCI101 reference -->
  <footer class="portfolio-footer">
    <p>© 2026 Prince Alfie Solomon | HCI101 Final Project</p>
  </footer>
</div>
</body>
</html>
