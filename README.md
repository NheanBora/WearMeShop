# Dentistry
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Dentistry - Smiles With Confident." />
  <link rel="icon" href="favicon.ico" type="image/x-icon" />
  <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
  
  <title>Wear Me Shop</title>

  <!-- Link your styles.css here -->
  <link rel="stylesheet" href="styles. css" />
</head>
<body>
  <header>
    <nav>
      <div class="logo">Denttistry</div>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
    <section class="hero">
      <h1>Welcome to Wear Me Shop</h1>
      <p>Smiles With Confident.</p>
      <button onclick="scrollToContact()">Shop Now</button>
    </section>
  </header>

  <main>
    <section id="about">
      <h2>About Us</h2>
      <p>The good smiles is a part of your life.</p>
    </section>

    <section id="products">
      <h2>Our Products</h2>
      <div class="gallery">
        <div class="card">Endodontics</div>
        <div class="card">Prosthodontics</div>
        <div class="card">Implantology</div>
        <div class="card">Surgery</div>
      </div>
    </section>

    <section id="contact">
      <h2>Contact Us</h2>
      <form onsubmit="submitForm(event)">
        <input type="text" placeholder="Nhean Bora" required />
        <input type="email" placeholder="nheanbora123@gmail.com" required />
        <textarea placeholder="Your Message" required></textarea>
        <button type="submit">Send</button>
      </form>
      <p class="form-status" id="form-status"></p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 WearMe Shop</p>
  </footer>

  <script>
    function scrollToContact() {
      const contactSection = document.getElementById("contact");
      contactSection.scrollIntoView({ behavior: "smooth" });
    }

    function submitForm(event) {
      event.preventDefault();
      document.getElementById("form-status").textContent = "Thank you! We'll contact you soon.";
    }
  </script>
</body>
</html>
