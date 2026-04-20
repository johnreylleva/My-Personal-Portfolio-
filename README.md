# My-Personal-Portfolio-
 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>John Rey Lleva | Aspiring Game Developer</title>

  <!-- Google Fonts + Font Awesome -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(145deg, #f0f4fc 0%, #e8eff9 100%);
      color: #1a2c3e;
      line-height: 1.5;
      padding: 2rem 1.5rem;
    }

    .container {
      max-width: 1050px;
      margin: 0 auto;
      background: #ffffff;
      border-radius: 2rem;
      box-shadow: 0 25px 45px -12px rgba(0, 0, 0, 0.15);
      overflow: hidden;
    }

    .inner-content {
      padding: 2rem 2.2rem 1.8rem 2.2rem;
    }

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

    .profile-img-wrapper {
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
    }

    .profile-img {
      width: 150px;
      height: 150px;
      object-fit: cover;
      object-position: center top;
      border-radius: 50%;
    }

    .profile-info { text-align: left; }

    .full-name {
      font-size: 2.1rem;
      font-weight: 800;
      background: linear-gradient(135deg, #1a4970, #2c6e9e);
      -webkit-background-clip: text;
      color: transparent;
    }

    .title-tag {
      font-size: 1.2rem;
      font-weight: 600;
      color: #2c6e9e;
      background: #eef3fc;
      padding: 0.4rem 1.2rem;
      border-radius: 60px;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
    }

    .section-title {
      font-size: 1.65rem;
      font-weight: 700;
      margin: 2rem 0 1rem 0;
      color: #1a4c6e;
      border-left: 5px solid #2c7ab1;
      padding-left: 1rem;
    }

    .about-text, .skills-container, .personal-card, .inspiration-block {
      background: #f6faff;
      border-radius: 1.5rem;
      padding: 1.3rem 1.8rem;
      border: 1px solid #e6edf8;
    }

    .info-table {
      width: 100%;
      border-collapse: collapse;
    }

    .info-table td {
      padding: 1rem;
      font-size: 0.98rem;
    }

    .skill-item {
      padding: 0.8rem 0;
      border-bottom: 1px solid #e4edf7;
    }

    .skill-name { font-weight: 700; }

    .footer-note {
      text-align: center;
      margin-top: 2rem;
      padding-top: 1rem;
      border-top: 1px solid #e2edf5;
      font-size: 0.85rem;
      color: #6f8eaa;
    }
  </style>
</head>

<body>

<div class="container">
  <div class="inner-content">

    <!-- PROFILE -->
    <header class="profile-section">
      <div class="profile-inner">

        <div class="profile-img-wrapper">
          <img src="Screenshot_20260420-205249_Gallery.jpg" alt="2x2 formal photo of John Rey Villanueva Lleva" class="profile-img">
        </div>

        <div class="profile-info">
          <h1 class="full-name">John Rey Villanueva Lleva</h1>
          <p class="title-tag"><i class="fas fa-gamepad"></i> ASPIRING GAME DEVELOPER</p>
        </div>

      </div>
    </header>

    <!-- ABOUT -->
    <section>
      <h2 class="section-title">About Me</h2>
      <div class="about-text">
        I am a dedicated first-year BSIT student at Our Lady of the Sacred Heart College of Guimba, passionate about technology and creativity.
      </div>
    </section>

    <!-- PERSONAL INFO -->
    <section>
      <h2 class="section-title">Personal Information</h2>
      <div class="personal-card">
        <table class="info-table">
          <tr><td>Full Name</td><td>John Rey Villanueva Lleva</td></tr>
          <tr><td>Age</td><td>18 Years Old</td></tr>
          <tr><td>Email</td><td>johnreylleva22@gmail.com</td></tr>
          <tr><td>Address</td><td>Guiset, Guimba, Nueva Ecija</td></tr>
        </table>
      </div>
    </section>

    <!-- SKILLS -->
    <section>
      <h2 class="section-title">Skills</h2>
      <div class="skills-container">
        <div class="skill-item"><span class="skill-name">Java:</span> Beginner</div>
        <div class="skill-item"><span class="skill-name">Python:</span> Beginner</div>
        <div class="skill-item"><span class="skill-name">HTML & CSS:</span> Intermediate</div>
      </div>
    </section>

    <!-- INSPIRATION -->
    <section>
      <h2 class="section-title">Inspiration</h2>
      <div class="inspiration-block">
        Inspired by Pokémon and its creator Satoshi Tajiri, I aim to create meaningful and creative games.
      </div>
    </section>

    <footer class="footer-note">
      © 2026 John Rey Villanueva Lleva
    </footer>

  </div>
</div>

</body>
</html>
