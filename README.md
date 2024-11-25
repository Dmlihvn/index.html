<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Artist Profile - Majish C">
  <title>Majish C - Artist Portfolio</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* Body background image */
    body {
      background-image: url('E6A60375-BAA4-4076-95A0-F4C870FDF889.png'); /* Updated image */
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      margin: 0;
      font-family: Arial, sans-serif;
      color: #fff;
    }

    /* Header Section (Hero) */
    .hero {
      background: rgba(0, 0, 0, 0.5); /* Dark overlay for text visibility */
      text-align: center;
      padding: 100px 0;
    }

    .hero h1 {
      font-size: 3em;
    }

    .hero p {
      font-size: 1.5em;
    }

    /* Navigation Bar */
    nav {
      background-color: rgba(0, 0, 0, 0.7);
      position: fixed;
      width: 100%;
      top: 0;
      left: 0;
      padding: 10px 0;
      z-index: 100;
    }

    nav ul {
      display: flex;
      justify-content: center;
      list-style: none;
      padding: 0;
      margin: 0;
    }

    nav ul li {
      margin: 0 15px;
    }

    nav ul li a {
      color: #fff;
      text-decoration: none;
      font-size: 1.2em;
    }

    /* About Section */
    #about {
      padding: 60px 20px;
      background-color: rgba(0, 0, 0, 0.6);
      color: #fff;
    }

    #about .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .about-image {
      width: 30%;
      border-radius: 10px;
    }

    .about-text {
      width: 60%;
    }

    /* Portfolio Section */
    #portfolio {
      padding: 60px 20px;
      background-color: rgba(0, 0, 0, 0.6);
      color: #fff;
    }

    .portfolio-filters {
      text-align: center;
      margin-bottom: 30px;
    }

    .filter-btn {
      padding: 10px 20px;
      background-color: #f1c40f;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin: 0 10px;
    }

    .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .portfolio-item {
      position: relative;
    }

    .portfolio-item img {
      width: 100%;
      border-radius: 10px;
      transition: transform 0.3s ease;
    }

    /* Make the recent artwork image bigger */
    .portfolio-item.recent img {
      width: 120%; /* Adjust size as needed */
      transform: scale(1.1); /* Slight zoom effect */
    }

    .overlay {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      color: #fff;
      text-align: center;
      padding: 10px;
    }

    /* Contact Section */
    #contact {
      padding: 60px 20px;
      background-color: rgba(0, 0, 0, 0.6);
      color: #fff;
    }

    .contact-form {
      display: flex;
      flex-direction: column;
    }

    .contact-form label {
      margin-bottom: 5px;
    }

    .contact-form input, .contact-form textarea {
      margin-bottom: 10px;
      padding: 10px;
      border-radius: 5px;
      border: none;
    }

    .contact-form button {
      padding: 10px 20px;
      background-color: #f1c40f;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background-color: rgba(0, 0, 0, 0.8);
    }

  </style>
</head>
<body>

  <!-- Header Section (Hero) -->
  <header class="hero">
    <div class="hero-overlay">
      <h1>Majish C</h1>
      <p>"Art is the only way to run away without leaving home."</p>
    </div>
  </header>

  <!-- Navigation Bar -->
  <nav>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#exhibitions">Exhibitions</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- About Section -->
  <section id="about" class="section">
    <div class="container">
      <!-- Updated Image for Artist Photo -->
      <img src="9C2BED12-4438-48AA-BC1B-C6C450E289B8.jpeg" alt="Artist Photo" class="about-image">
      <div class="about-text">
        <h2>About Me</h2>
        <p>
          I am an artist whose work is inspired by the intersection of nature and technology. My art explores themes of transformation, environment, and the impact of the digital world on organic life.
        </p>
      </div>
    </div>
  </section>

  <!-- Portfolio Section -->
  <section id="portfolio" class="section">
    <h2>Portfolio</h2>
    <div class="portfolio-filters">
      <button class="filter-btn" data-category="recent">Recent Works</button>
      <button class="filter-btn" data-category="digital">Digital Art</button>
      <button class="filter-btn" data-category="all">All</button>
    </div>
    <div class="portfolio-grid">
      <div class="portfolio-item digital">
        <img src="digital-art1.jpg" alt="Digital Artwork 1">
        <div class="overlay">
          <p>Digital Art - 2024</p>
        </div>
      </div>
      <div class="portfolio-item recent">
        <!-- Updated image as per your request -->
        <img src="E6A60375-BAA4-4076-95A0-F4C870FDF889.png" alt="Recent Artwork 1">
        <div class="overlay">
          <p>Recent Work - 2024</p>
        </div>
      </div>
      <div class="portfolio-item digital">
        <img src="digital-art2.jpg" alt="Digital Artwork 2">
        <div class="overlay">
          <p>Digital Art - 2023</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Exhibitions Section -->
  <section id="exhibitions" class="section">
    <h2>Exhibitions</h2>
    <div class="exhibition-list">
      <div class="exhibition-item">
        <h3>Solo Show at Art Gallery</h3>
        <p>January 2024, New York</p>
      </div>
      <!-- More exhibitions can go here -->
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="section">
    <h2>Contact</h2>
    <form action="#" method="POST" class="contact-form">
      <label for="name">Name</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email</label>
      <input type="email" id="email" name="email" required>

      <label for="message">Message</label>
      <textarea id="message" name="message" rows="4" required></textarea>

      <button type="submit">Send Message</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2024 Majish C. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>

</body>
</html>
