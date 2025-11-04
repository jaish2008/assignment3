<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Golden Slice | Pizza Service</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">

<script>
// Smooth scroll to sections
function scrollToSection(id) {
  document.getElementById(id).scrollIntoView({ behavior: 'smooth' });
}

// Simple contact form message
document.getElementById('contactForm').addEventListener('submit', (e) => {
  e.preventDefault();
  document.getElementById('formMsg').textContent = "✅ Thank you! We'll get back to you soon.";
  e.target.reset();
});


</script>
</head>

<body>
  <!-- Navbar -->
  <header class="navbar">
    <div class="logo">🍕 Golden Slice</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#services">Menu</a>
      <a href="#steps">How to Order</a>
      <a href="#reviews">Reviews</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
    <button class="order-btn" onclick="scrollToSection('contact')">Order Now</button>
  </header>

  <!-- Hero Section -->
  <section id="home" class="hero">
    <div class="hero-content">
      <h1>Fresh. Hot. Golden.</h1>
      <p>Experience premium pizzas made with passion, baked to perfection, and delivered with love.</p>
      <button onclick="scrollToSection('services')">Explore Menu</button>
    </div>
  </section>

  <!-- Description / Why Us -->
  <section class="why-us">
    <div class="why-content">
      <h2>Why Choose Golden Slice?</h2>
      <div class="why-grid">
        <div class="why-card">
          <h3>🔥 Fresh Ingredients</h3>
          <p>We use farm-fresh veggies and hand-tossed dough daily.</p>
        </div>
        <div class="why-card">
          <h3>⚡ Fast Delivery</h3>
          <p>Hot pizza at your door in under 30 minutes.</p>
        </div>
        <div class="why-card">
          <h3>💛 Great Deals</h3>
          <p>Save more with combo offers and daily discounts.</p>
        </div>
        <div class="why-card">
          <h3>🍴 Variety</h3>
          <p>Choose from over 20 pizzas with custom toppings.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Services (Menu) -->
  <section id="services" class="services">
    <h2>Our Great Deals</h2>
    <div class="menu-scroll">
      <div class="menu-card">
        <img src="margherita.png" alt="Margherita Pizza">
        <h3>Margherita</h3>
        <p>Classic cheese, tomato & basil</p>
        <span>$9.99</span>
      </div>
      <div class="menu-card">
        <img src="pepperoni.png" alt="Pepperoni Pizza">
        <h3>Pepperoni</h3>
        <p>Loaded with crispy pepperoni</p>
        <span>$11.49</span>
      </div>
      <div class="menu-card">
        <img src="veggoe supreme.png" alt="Veggie Pizza">
        <h3>Veggie Supreme</h3>
        <p>Fresh veggies with extra cheese</p>
        <span>$10.99</span>
      </div>
      <div class="menu-card">
        <img src="https://images.unsplash.com/photo-1550547660-d9450f859349" alt="BBQ Pizza">
        <h3>BBQ Chicken</h3>
        <p>Smoky BBQ sauce with chicken</p>
        <span>$12.49</span>
      </div>
    </div>
  </section>

  <!-- Ordering Steps -->
  <section id="steps" class="steps">
    <h2>How to Order</h2>
    <div class="steps-container">
      <div class="step">
        <h3>1️⃣ Choose Your Pizza</h3>
        <p>Pick from our menu or customize your own.</p>
      </div>
      <div class="step">
        <h3>2️⃣ Place Your Order</h3>
        <p>Quick and easy checkout experience.</p>
      </div>
      <div class="step">
        <h3>3️⃣ Get It Delivered</h3>
        <p>Our delivery heroes bring it hot and fresh!</p>
      </div>
    </div>
  </section>

  <!-- Customer Reviews -->
  <section id="reviews" class="reviews">
    <h2>What Our Customers Say</h2>
    <div class="review-cards">
      <div class="review-card">
        <p>"Best pizza I’ve ever had! Crispy crust and perfect cheese blend."</p>
        <span>- Sarah J.</span>
      </div>
      <div class="review-card">
        <p>"Fast delivery and absolutely delicious! Highly recommend."</p>
        <span>- Mike D.</span>
      </div>
      <div class="review-card">
        <p>"Golden Slice never disappoints. Great quality and taste!"</p>
        <span>- Priya K.</span>
      </div>
    </div>
  </section>

  <!-- About Us -->
  <section id="about" class="about">
    <div class="about-content">
      <img src="about.png" alt="About Pizza Haven">
      <div>
        <h2>About Golden Slice</h2>
        <p>At Golden Slice, we believe every slice tells a story. Our chefs craft pizzas using traditional recipes with a modern twist. Whether dine-in or delivery, we promise freshness, flavor, and satisfaction in every bite.</p>
      </div>
    </div>
  </section>

  <!-- Contact Us -->
  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <form id="contactForm">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p id="formMsg"></p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 Golden Slice | Designed with ❤️ and Cheese.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
<style>

    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; }

body {
  background-color: #000;
  color: #fff;
  scroll-behavior: smooth;
}

/* Navbar */
.navbar {
  display: flex; justify-content: space-between; align-items: center;
  padding: 15px 50px;
  background: rgba(0,0,0,0.8);
  position: fixed; top: 0; width: 100%;
  z-index: 10; backdrop-filter: blur(10px);
}

.logo { color: #FFD700; font-weight: 700; font-size: 1.5em; }
nav a {
  color: #fff; text-decoration: none; margin: 0 15px; transition: color 0.3s;
}
nav a:hover { color: #FFD700; }
.order-btn {
  background: #FFD700; color: #000; border: none; padding: 10px 20px;
  border-radius: 20px; font-weight: 600; cursor: pointer;
  transition: transform 0.3s, box-shadow 0.3s;
}
.order-btn:hover {
  transform: scale(1.05);
  box-shadow: 0 0 10px #FFD700;
}

/* Hero Section */
.hero {
  height: 100vh;
  background: url('https://images.unsplash.com/photo-1601924582971-c9f6c2e6c9d8') center/cover no-repeat;
  display: flex; justify-content: center; align-items: center; text-align: center;
  position: relative;
}
.hero::before {
  content: ""; position: absolute; inset: 0; background: rgba(0,0,0,0.5);
}
.hero-content {
  position: relative; z-index: 1; max-width: 600px;
}
.hero h1 { font-size: 3em; color: #FFD700; margin-bottom: 15px; animation: fadeInDown 1s; }
.hero p { font-size: 1.2em; margin-bottom: 25px; animation: fadeInUp 1s; }
.hero button {
  background: #FFD700; color: #000; padding: 12px 25px; border: none;
  border-radius: 30px; font-weight: 600; cursor: pointer;
  transition: 0.3s;
}
.hero button:hover { background: #e6c200; }

/* Why Us Section */
.why-us {
  padding: 80px 50px; background: #111;
}
.why-us h2 { text-align: center; color: #FFD700; margin-bottom: 40px; }
.why-grid {
  display: flex; flex-wrap: wrap; gap: 30px; justify-content: center;
}
.why-card {
  background: #222; padding: 30px; border-radius: 10px;
  width: 250px; text-align: center; transition: transform 0.3s;
}
.why-card:hover { transform: translateY(-10px); }

/* Services */
.services { padding: 80px 50px; background: #000; text-align: center; }
.services h2 { color: #FFD700; margin-bottom: 30px; }
.menu-scroll {
  display: flex; gap: 30px; overflow-x: auto; padding-bottom: 10px;
  scrollbar-width: none;
}
.menu-scroll::-webkit-scrollbar { display: none; }
.menu-card {
  background: #111; border-radius: 10px; padding: 15px; min-width: 250px;
  transition: transform 0.3s;
}
.menu-card:hover { transform: scale(1.05); }
.menu-card img { width: 100%; height: 180px; border-radius: 10px; object-fit: cover; }
.menu-card h3 { color: #FFD700; margin-top: 10px; }
.menu-card span { color: #FFD700; font-weight: bold; }

/* Steps */
.steps { padding: 80px 50px; background: #111; text-align: center; }
.steps h2 { color: #FFD700; margin-bottom: 40px; }
.steps-container {
  display: flex; justify-content: center; flex-wrap: wrap; gap: 30px;
}
.step {
  background: #000; border: 1px solid #FFD700; border-radius: 10px;
  padding: 20px; width: 250px; transition: transform 0.3s;
}
.step:hover { transform: translateY(-10px); }

/* Reviews */
.reviews { background: #000; padding: 80px 50px; text-align: center; }
.reviews h2 { color: #FFD700; margin-bottom: 40px; }
.review-cards {
  display: flex; flex-wrap: wrap; justify-content: center; gap: 30px;
}
.review-card {
  background: #111; border-radius: 10px; padding: 25px; width: 280px;
  border-left: 3px solid #FFD700;
}

/* About */
.about { background: #111; padding: 80px 50px; }
.about-content {
  display: flex; align-items: center; gap: 40px; flex-wrap: wrap;
}
.about-content img {
  width: 400px; border-radius: 10px; border: 3px solid #FFD700;
}
.about-content h2 { color: #FFD700; margin-bottom: 15px; }

/* Contact */
.contact { background: #000; padding: 80px 50px; text-align: center; }
.contact h2 { color: #FFD700; margin-bottom: 30px; }
form {
  display: flex; flex-direction: column; align-items: center; gap: 15px;
}
form input, form textarea {
  width: 300px; padding: 10px; border: none; border-radius: 5px;
}
form button {
  background: #FFD700; color: #000; padding: 10px 20px; border: none;
  border-radius: 25px; cursor: pointer; transition: 0.3s;
}
form button:hover { background: #e6c200; }
#formMsg { margin-top: 10px; color: #0f0; }

/* Footer */
footer {
  background: #111; text-align: center; padding: 20px;
  color: #FFD700; font-size: 0.9em;
}

/* Animations */
@keyframes fadeInDown { from { opacity: 0; transform: translateY(-20px);} to {opacity:1; transform:translateY(0);} }
@keyframes fadeInUp { from { opacity: 0; transform: translateY(20px);} to {opacity:1; transform:translateY(0);} }

</style>
