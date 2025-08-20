# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
# HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BUYME</title>
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>

<header>
  <div class="container header-flex">
    <div class="logo">BUYMe</div>
    <nav class="nav-flex">
      <a href="#home">HOME</a>
      <a href="#about">ABOUT</a>
      <a href="#services">SERVICES</a>
      <a href="#electronics">ELECTRONICS</a>
      <a href="#contact">CONTACT</a>
    </nav>
    <input type="text" placeholder="Search products..." class="search-bar">
    <div class="cart"><i class="fas fa-shopping-cart"></i> Cart</div>
  </div>
</header>

<section id="home" class="hero-banner">
  <img src="banner.webp" alt="Electronics Banner">
  <div class="hero-text-overlay">
    <h1>Welcome to BUYMe</h1>
    <p>Your one-stop shop for the latest electronics</p>
    <a href="#electronics" class="btn">Shop Now</a>
  </div>
</section>

<section id="about" class="section-flex">
  <div class="container">
    <h2>ABOUT</h2>
    <p>BUYMe is your premier destination for cutting-edge electronics. We provide laptops, smartphones, cameras, and more with unbeatable prices and service.</p>
  </div>
</section>

<section id="services" class="section-flex services-flex">
  <div class="container">
    <h2>OUR SERVICES</h2>
    <div class="services-grid">
      <div class="service-card">
        <i class="fas fa-shipping-fast fa-3x"></i>
        <h3>FAST SHIPPING</h3>
        <p>Get your products delivered quickly and safely.</p>
      </div>
      <div class="service-card">
        <i class="fas fa-headset fa-3x"></i>
        <h3>24/7 SUPPORT</h3>
        <p>Our team is available around the clock for any queries.</p>
      </div>
      <div class="service-card">
        <i class="fas fa-shield-alt fa-3x"></i>
        <h3>SECURE PAYMENTS</h3>
        <p>All transactions are safe and encrypted.</p>
      </div>
    </div>
  </div>
</section>

<section id="electronics" class="section-flex">
  <div class="container">
    <h2>POPULAR BUYS OF THE WEEK</h2>
    <div class="products-grid">
      <div class="product-card">
        <img src="633adbc8d9f918464775a999-asus-rog-strix-scar-15-2022-gaming.jpg" alt="Laptop">
        <h3>ASUS ROG STRIX</h3>
        <p class="price">74,190</p>
        <button class="btn">Buy Now</button>
      </div>
      <div class="product-card">
        <img src="NBXTGooPix9Pro5GVar_1_1.webp" alt="Smartphone">
        <h3>GOOGLE PIXEL 9 PRO</h3>
        <p class="price">79,000</p>
        <button class="btn">Buy Now</button>
      </div>
      <div class="product-card">
        <img src="jbl tune 770nc.jpg" alt="Headphones">
        <h3>JBL TUNE 7770NC</h3>
        <p class="price">4,599</p>
        <button class="btn">Buy Now</button>
      </div>
      <div class="product-card">
        <img src="APPLE WATCH ULTRA 2.jpg" alt="Smartwatch">
        <h3>APPLE WATCH ULTRA 2</h3>
        <p class="price">81,099</p>
        <button class="btn">Buy Now</button>
      </div>
    </div>
  </div>
</section>

<section id="contact" class="section-flex">
  <div class="container">
    <h2>Contact Us</h2>
    <p>Email: support@buyme.com | Phone: 091 346 4337</p>
    <p>Follow us on social media: 
      <i class="fab fa-facebook-square"></i> 
      <i class="fab fa-twitter-square"></i> 
      <i class="fab fa-instagram-square"></i>
    </p>
  </div>
</section>

<footer class="footer-flex">
  <div class="container">
    <p>&copy; 2025 BUYMe. All Rights Reserved.</p>
  </div>
</footer>

</body>
</html>
```
#CSS
```

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: "Arial", sans-serif;
  background: #9ee5f1;
  color: #333;
  font-size: 18px;
}

header {
  background: #050506;
  color: #0b0b0b;
  padding: 10px 0;
  position: sticky;
  top: 0;
  z-index: 100;
}
.header-flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 90%;
  max-width: 1200px;
  margin: auto;
}
.logo {
  font-size: 2rem;
  font-weight: bold;
  color: #fffffc;
}
.nav-flex a {
  margin: 0 15px;
  color: #f8a5a5;
  text-decoration: none;
  font-weight: bold;
}
.nav-flex a:hover {
  text-decoration: underline;
}
.search-bar {
  padding: 8px 12px;
  border-radius: 5px;
  border: none;
  width: 200px;
}
.cart {
  color: #f6f5f3;
  font-weight: bold;
  cursor: pointer;
}

.hero-banner {
  position: relative;
  text-align: center;
}
.hero-banner img {
  width: 100%;
  max-height: 400px;
  object-fit: cover;
}
.hero-text-overlay {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: #030202;
}
.hero-text-overlay h1 {
  font-size: 3rem;
  margin-bottom: 10px;
}
.hero-text-overlay p {
  font-size: 1.5rem;
  margin-bottom: 15px;
}
.hero-text-overlay .btn {
  padding: 12px 25px;
  background: #ff9900;
  color: #131921;
  border: none;
  border-radius: 25px;
  cursor: pointer;
  font-weight: bold;
}
.hero-text-overlay .btn:hover {
  background: #e68a00;
}

.section-flex {
  padding: 60px 0;
  text-align: center;
}
.section-flex h2 {
  font-size: 2.5rem;
  margin-bottom: 40px;
  color: #030609;
}
.section-flex p {
  font-size: 1.2rem;
  max-width: 800px;
  margin: auto;
  line-height: 1.6;
}

.services-flex .services-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}
.service-card {
  background: #14abfc;
  padding: 20px;
  flex: 1;
  min-width: 220px;
  max-width: 300px;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  text-align: center;
  transition: transform 0.3s;
}
.service-card i {
  color: #f3f38e;
  margin-bottom: 10px;
}
.service-card h3 {
  font-size: 1.3rem;
  margin-bottom: 10px;
}
.service-card p {
  font-size: 1rem;
}
.service-card:hover {
  transform: translateY(-5px);
}

.products-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  gap: 20px;
}
.product-card {
  background: #f6f8f9;
  padding: 15px;
  flex: 1;
  min-width: 220px;
  max-width: 250px;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  text-align: center;
  transition: transform 0.3s;
}
.product-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 8px;
  margin-bottom: 10px;
}
.product-card h3 {
  font-size: 1.3rem;
  margin-bottom: 10px;
  color: #05080b;
}
.product-card .price {
  font-weight: bold;
  font-size: 1.2rem;
  color: #f23e07;
  margin-bottom: 10px;
}
.product-card button {
  padding: 10px 15px;
  font-size: 1rem;
  border: none;
  background: #8ce2f6;
  color: #131921;
  border-radius: 25px;
  cursor: pointer;
  font-weight: bold;
}
.product-card button:hover {
  background: #e68a00;
}
.product-card:hover {
  transform: translateY(-5px);
}

#contact p {
  font-size: 1.2rem;
  margin-bottom: 10px;
}

.footer-flex {
  background: #131921;
  color: #fff;
  text-align: center;
  padding: 25px;
  font-size: 1.1rem;
}

@media(max-width: 768px) {
  .products-grid, .services-grid {
    flex-direction: column;
    align-items: center;
  }
  .hero-text-overlay h1 {
    font-size: 2rem;
  }
  .hero-text-overlay p {
    font-size: 1.2rem;
  }
  .search-bar {
    width: 150px;
  }
}
```
## OUTPUT
<img width="1918" height="1078" alt="SS1" src="https://github.com/user-attachments/assets/b6adc0f0-2d6a-4dc9-a882-9f9c5f32a4ba" />
<img width="1918" height="1078" alt="SS2" src="https://github.com/user-attachments/assets/aa0fdbae-0a8f-46a7-a748-01db44a0381a" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.

