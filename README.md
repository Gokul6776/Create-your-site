<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>CSS Final Project - One Page</title>
  <style>
    /* Skip link */
    .skip-link {
      position: absolute;
      top: -40px;
      left: 0;
      background: #000;
      color: #fff;
      padding: 8px;
      z-index: 100;
    }
    .skip-link:focus {
      top: 0;
    }

    /* Navigation with flex */
    .nav {
      display: flex;
      list-style: none;
      background-color: #333;
      padding: 10px;
      margin: 0;
    }
    .nav li {
      margin: 0 15px;
    }
    .nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    .nav a:hover {
      text-decoration: underline;
      color: yellow;
    }

    /* Images styled with box model */
    img {
      border: 3px solid #333;
      padding: 10px;
      border-radius: 10px;
      margin: 10px;
      width: 200px;
    }

    /* Grid layout */
    .grid-gallery {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
      padding: 20px;
    }

    /* nth-child example */
    .grid-gallery img:nth-child(even) {
      border-radius: 50%;
    }

    /* Hover effect */
    img:hover {
      transform: scale(1.05);
      transition: transform 0.3s ease-in-out;
    }

    /* Page sections */
    section {
      padding: 20px;
    }

    h2 {
      border-bottom: 2px solid #ccc;
      padding-bottom: 5px;
    }
  </style>
</head>
<body>

  <a href="#main" class="skip-link">Skip to Main Content</a>

  <nav>
    <ul class="nav">
      <li><a href="#home">Home</a></li>
      <li><a href="#gallery">Gallery</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <main id="main">
    
    <!-- Home Section -->
    <section id="home">
      <h2>🏠 Home</h2>
      <p>Welcome to my CSS final project all-in-one webpage!</p>
      <img src="https://via.placeholder.com/200?text=Home+Image" alt="Welcome image" />
    </section>

    <!-- Gallery Section -->
    <section id="gallery">
      <h2>🖼️ Image Gallery</h2>
      <div class="grid-gallery">
        <img src="https://via.placeholder.com/200?text=Image+1" alt="Gallery 1">
        <img src="https://via.placeholder.com/200?text=Image+2" alt="Gallery 2">
        <img src="https://via.placeholder.com/200?text=Image+3" alt="Gallery 3">
        <img src="https://via.placeholder.com/200?text=Image+4" alt="Gallery 4">
        <img src="https://via.placeholder.com/200?text=Image+5" alt="Gallery 5">
        <img src="https://via.placeholder.com/200?text=Image+6" alt="Gallery 6">
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
      <h2>📞 Contact</h2>
      <p>You can email me at <a href="mailto:example@email.com">example@email.com</a></p>
      <img src="https://via.placeholder.com/200?text=Contact+Image" alt="Contact" />
    </section>

  </main>

</body>
</html>
