# Ex02 Commercial Website
## Date: 31-10-2026

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
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Checkmate Guild | Premium Chess Gear & Services</title>
  <!-- Google Fonts & FontAwesome -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;700;800&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <!-- Link to External CSS -->
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- NAVIGATION BAR -->
  <header class="header">
    <div class="nav-container">
      <a href="#home" class="logo">
        <i class="fa-solid fa-chess-knight"></i>
        <span>CHECKMATE GUILD</span>
      </a>
      <ul class="nav-links">
        <li><a href="#home" class="active">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#account">Account</a></li>
      </ul>
      <div class="nav-actions">
        <button class="cart-btn" onclick="toggleCart()">
          <i class="fa-solid fa-shopping-bag"></i>
          <span class="cart-badge" id="cartCount">2</span>
        </button>
      </div>
    </div>
  </header>

  <!-- HOMEPAGE SECTION -->
  <section id="home" class="hero">
    <div class="hero-content">
      <div class="hero-tag">
        <i class="fa-solid fa-crown"></i> Official FIDE Supplier
      </div>
      <h1 class="hero-title">Master the Board with <span>Grandmaster</span> Precision</h1>
      <p class="hero-desc">Discover handcrafted luxury Staunton sets, digital tournament clocks, and elite training literature for serious players.</p>
      <div class="hero-btns">
        <a href="#products" class="btn btn-primary"><i class="fa-solid fa-chess"></i> Explore Shop</a>
        <a href="#about" class="btn btn-secondary">Learn Story</a>
      </div>
    </div>
    <div class="hero-image">
      <div class="hero-card">
        <i class="fa-solid fa-chess-king"></i>
        <h3 class="brand-font">Heritage Staunton No. 6</h3>
        <p style="color: var(--text-muted); margin: 0.5rem 0 1rem; font-size: 0.9rem;">Triple-Weighted Ebony & Boxwood</p>
        <span class="product-price">$249.00</span>
      </div>
    </div>
  </section>

  <!-- PRODUCTS SECTION -->
  <section id="products">
    <div class="section-header">
      <h2>Featured Gear & Services</h2>
      <p>Precision-engineered equipment approved for International FIDE competitions.</p>
    </div>
    <div class="product-grid">
      <!-- Product 1 -->
      <div class="product-card">
        <div class="product-img"><i class="fa-solid fa-chess-board"></i></div>
        <div class="product-info">
          <div>
            <div class="product-title">Luxury Mahogany Board</div>
            <p style="color:var(--text-muted); font-size:0.85rem;">2.25 inch tournament squares</p>
          </div>
          <div class="product-meta">
            <span class="product-price">$129.00</span>
            <button class="btn btn-primary" style="padding: 0.5rem 1rem;" onclick="toggleCart()">Add</button>
          </div>
        </div>
      </div>
      <!-- Product 2 -->
      <div class="product-card">
        <div class="product-img"><i class="fa-solid fa-stopwatch"></i></div>
        <div class="product-info">
          <div>
            <div class="product-title">DGT 2010 Digital Clock</div>
            <p style="color:var(--text-muted); font-size:0.85rem;">FIDE Approved timer preset modes</p>
          </div>
          <div class="product-meta">
            <span class="product-price">$89.50</span>
            <button class="btn btn-primary" style="padding: 0.5rem 1rem;" onclick="toggleCart()">Add</button>
          </div>
        </div>
      </div>
      <!-- Product 3 -->
      <div class="product-card">
        <div class="product-img"><i class="fa-solid fa-book-open"></i></div>
        <div class="product-info">
          <div>
            <div class="product-title">Grandmaster Openings Vol. 1</div>
            <p style="color:var(--text-muted); font-size:0.85rem;">Hardcover masterclass guide</p>
          </div>
          <div class="product-meta">
            <span class="product-price">$45.00</span>
            <button class="btn btn-primary" style="padding: 0.5rem 1rem;" onclick="toggleCart()">Add</button>
          </div>
        </div>
      </div>
      <!-- Product 4 -->
      <div class="product-card">
        <div class="product-img"><i class="fa-solid fa-graduation-cap"></i></div>
        <div class="product-info">
          <div>
            <div class="product-title">1-on-1 GM Coaching</div>
            <p style="color:var(--text-muted); font-size:0.85rem;">60-minute interactive game analysis</p>
          </div>
          <div class="product-meta">
            <span class="product-price">$120.00</span>
            <button class="btn btn-primary" style="padding: 0.5rem 1rem;" onclick="alert('Coaching session booked!')">Book</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT US SECTION -->
  <section id="about">
    <div class="about-container">
      <div class="about-text">
        <div class="hero-tag"><i class="fa-solid fa-shield-halved"></i> Excellence Since 2012</div>
        <h2>Crafting Royal Equipment for Chess Connoisseurs</h2>
        <p>Checkmate Guild was founded by international masters with a single mission: to create competition-grade chess sets that blend artisan woodwork with modern tournament precision.</p>
        <div class="about-stats">
          <div class="stat-box">
            <span class="stat-number">50K+</span>
            <span class="stat-label">Boards Shipped</span>
          </div>
          <div class="stat-box">
            <span class="stat-number">100%</span>
            <span class="stat-label">FIDE Compliant</span>
          </div>
          <div class="stat-box">
            <span class="stat-number">4.9★</span>
            <span class="stat-label">User Rating</span>
          </div>
        </div>
      </div>
      <div class="about-visual">
        <i class="fa-solid fa-chess-rook"></i>
      </div>
    </div>
  </section>

  <!-- CONTACT & USER ACCOUNT SECTION -->
  <section id="contact">
    <div class="section-header">
      <h2>Contact & User Portal</h2>
      <p>Connect with our chess equipment experts or access your member account.</p>
    </div>
    <div class="form-flex-container">
      <!-- Contact Form -->
      <div class="form-card">
        <h3><i class="fa-solid fa-envelope-open-text" style="color: var(--gold-primary);"></i> Get in Touch</h3>
        <div class="form-group">
          <label>Full Name</label>
          <input type="text" placeholder="e.g., Garry Kasparov">
        </div>
        <div class="form-group">
          <label>Email Address</label>
          <input type="email" placeholder="name@example.com">
        </div>
        <div class="form-group">
          <label>Inquiry Message</label>
          <textarea rows="4" placeholder="How can we help you today?"></textarea>
        </div>
        <button class="btn btn-primary" onclick="alert('Message Sent!')">Send Message</button>
      </div>

      <!-- User Account Form -->
      <div class="form-card" id="account">
        <h3><i class="fa-solid fa-user-shield" style="color: var(--gold-primary);"></i> Member Portal</h3>
        <div class="form-group">
          <label>Username or FIDE ID</label>
          <input type="text" placeholder="Enter your username">
        </div>
        <div class="form-group">
          <label>Password</label>
          <input type="password" placeholder="••••••••">
        </div>
        <div style="display: flex; justify-content: space-between; align-items: center; font-size: 0.85rem; color: var(--text-muted);">
          <label><input type="checkbox"> Remember me</label>
          <a href="#" style="color: var(--gold-primary);">Forgot password?</a>
        </div>
        <button class="btn btn-primary" onclick="alert('Logged in successfully!')">Sign In</button>
        <button class="btn btn-secondary" onclick="alert('Registration form opened!')">Create New Account</button>
      </div>
    </div>
  </section>

  <!-- FOOTER SECTION -->
  <footer class="footer">
    <div class="footer-container">
      <div class="footer-col">
        <div class="logo">
          <i class="fa-solid fa-chess-knight"></i>
          <span>CHECKMATE GUILD</span>
        </div>
        <p style="color: var(--text-muted); font-size: 0.9rem;">
          Premier destination for luxury chess sets, tournament clocks, and grandmaster literature.
        </p>
      </div>
      <div class="footer-col">
        <h4>Navigation</h4>
        <ul class="footer-links">
          <li><a href="#home">Home</a></li>
          <li><a href="#products">Shop Products</a></li>
          <li><a href="#about">About Our Craft</a></li>
          <li><a href="#contact">Support Contact</a></li>
        </ul>
      </div>
      <div class="footer-col">
        <h4>Connect With Us</h4>
        <div class="social-links">
          <a href="#" class="social-btn"><i class="fa-brands fa-github"></i></a>
          <a href="#" class="social-btn"><i class="fa-brands fa-linkedin"></i></a>
          <a href="#" class="social-btn"><i class="fa-brands fa-x-twitter"></i></a>
          <a href="#" class="social-btn"><i class="fa-brands fa-youtube"></i></a>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; 2026 Checkmate Guild Inc. All rights reserved.</p>
      <p>Designed with CSS Flexbox Layout</p>
    </div>
  </footer>

  <!-- INTERACTIVE CART OVERLAY & DRAWER -->
  <div class="cart-overlay" id="cartOverlay" onclick="toggleCart()"></div>

  <div class="cart-drawer" id="cartDrawer">
    <div class="cart-header">
      <h3><i class="fa-solid fa-shopping-bag"></i> Your Cart</h3>
      <button class="close-cart-btn" onclick="toggleCart()">&times;</button>
    </div>
    
    <div class="cart-body">
      <div class="cart-item">
        <div>
          <div class="cart-item-title">Heritage Staunton No. 6</div>
          <div class="cart-item-price">$249.00</div>
        </div>
        <span class="cart-item-qty">x1</span>
      </div>
      <div class="cart-item">
        <div>
          <div class="cart-item-title">DGT 2010 Digital Clock</div>
          <div class="cart-item-price">$89.50</div>
        </div>
        <span class="cart-item-qty">x1</span>
      </div>
    </div>

    <div class="cart-footer">
      <div class="cart-total">
        <span>Total:</span>
        <span>$338.50</span>
      </div>
      <button class="btn btn-primary" style="width: 100%; justify-content: center;" onclick="alert('Proceeding to Checkout!')">
        Checkout
      </button>
    </div>
  </div>

  <script>
    function toggleCart() {
      document.getElementById('cartDrawer').classList.toggle('active');
      document.getElementById('cartOverlay').classList.toggle('active');
    }
  </script>

</body>
</html>
/* ==========================================
   GLOBAL STYLES & VARIABLES
   ========================================== */
:root {
  --bg-main: #0e1117;
  --bg-card: #161b22;
  --bg-accent: #21262d;
  --gold-primary: #d4af37;
  --gold-hover: #f3cf65;
  --text-main: #f0f6fc;
  --text-muted: #8b949e;
  --border-color: #30363d;
  --shadow-glow: 0 10px 30px rgba(212, 175, 55, 0.15);
  --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Plus Jakarta Sans', sans-serif;
  background-color: var(--bg-main);
  color: var(--text-main);
  line-height: 1.6;
}

h1, h2, h3, h4, .brand-font {
  font-family: 'Cinzel', serif;
  letter-spacing: 0.5px;
}

a {
  text-decoration: none;
  color: inherit;
  transition: var(--transition);
}

/* ==========================================
   FLEXBOX NAVIGATION BAR
   ========================================== */
.header {
  position: sticky;
  top: 0;
  z-index: 1000;
  background: rgba(14, 17, 23, 0.9);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--border-color);
}

.nav-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem 1.5rem;
  display: flex; /* FLEXBOX */
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  font-size: 1.4rem;
  font-weight: 700;
  color: var(--gold-primary);
}

.logo i {
  font-size: 1.8rem;
}

.nav-links {
  display: flex; /* FLEXBOX */
  list-style: none;
  gap: 2rem;
  align-items: center;
}

.nav-links a {
  font-size: 0.95rem;
  font-weight: 500;
  color: var(--text-muted);
}

.nav-links a:hover,
.nav-links a.active {
  color: var(--gold-primary);
}

.nav-actions {
  display: flex;
  align-items: center;
  gap: 1.25rem;
}

.cart-btn {
  position: relative;
  background: var(--bg-accent);
  border: 1px solid var(--border-color);
  color: var(--text-main);
  width: 42px;
  height: 42px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: var(--transition);
}

.cart-btn:hover {
  border-color: var(--gold-primary);
  color: var(--gold-primary);
}

.cart-badge {
  position: absolute;
  top: -4px;
  right: -4px;
  background: var(--gold-primary);
  color: #000;
  font-size: 0.75rem;
  font-weight: 700;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* ==========================================
   HERO SECTION (FLEXBOX)
   ========================================== */
.hero {
  max-width: 1200px;
  margin: 0 auto;
  padding: 5rem 1.5rem;
  display: flex; /* FLEXBOX */
  align-items: center;
  justify-content: space-between;
  gap: 3rem;
  min-height: 80vh;
}

.hero-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.hero-tag {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: rgba(212, 175, 55, 0.1);
  border: 1px solid rgba(212, 175, 55, 0.3);
  color: var(--gold-primary);
  padding: 0.4rem 1rem;
  border-radius: 50px;
  font-size: 0.85rem;
  font-weight: 600;
  width: fit-content;
}

.hero-title {
  font-size: 3.2rem;
  line-height: 1.15;
  color: var(--text-main);
}

.hero-title span {
  color: var(--gold-primary);
}

.hero-desc {
  color: var(--text-muted);
  font-size: 1.1rem;
  max-width: 520px;
}

.hero-btns {
  display: flex; /* FLEXBOX */
  gap: 1rem;
  margin-top: 0.5rem;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.85rem 1.8rem;
  border-radius: 8px;
  font-weight: 600;
  cursor: pointer;
  transition: var(--transition);
  border: none;
}

.btn-primary {
  background: var(--gold-primary);
  color: #000;
}

.btn-primary:hover {
  background: var(--gold-hover);
  transform: translateY(-2px);
  box-shadow: var(--shadow-glow);
}

.btn-secondary {
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  color: var(--text-main);
}

.btn-secondary:hover {
  border-color: var(--gold-primary);
  color: var(--gold-primary);
}

.hero-image {
  flex: 1;
  display: flex;
  justify-content: center;
  position: relative;
}

.hero-card {
  width: 100%;
  max-width: 440px;
  background: linear-gradient(145deg, var(--bg-card), var(--bg-accent));
  border: 1px solid var(--border-color);
  border-radius: 16px;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.5);
}

.hero-card i {
  font-size: 5rem;
  color: var(--gold-primary);
  margin-bottom: 1rem;
}

/* ==========================================
   SECTION CONTAINERS & HEADERS
   ========================================== */
section {
  padding: 5rem 1.5rem;
  max-width: 1200px;
  margin: 0 auto;
}

.section-header {
  text-align: center;
  margin-bottom: 3.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.5rem;
}

.section-header h2 {
  font-size: 2.2rem;
  color: var(--text-main);
}

.section-header p {
  color: var(--text-muted);
  max-width: 600px;
}

/* ==========================================
   PRODUCTS SECTION (FLEXBOX GRID)
   ========================================== */
.product-grid {
  display: flex; /* FLEXBOX */
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
}

.product-card {
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  border-radius: 12px;
  width: 270px;
  display: flex; /* FLEXBOX */
  flex-direction: column;
  overflow: hidden;
  transition: var(--transition);
}

.product-card:hover {
  transform: translateY(-8px);
  border-color: var(--gold-primary);
  box-shadow: var(--shadow-glow);
}

.product-img {
  height: 200px;
  background: var(--bg-accent);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 4.5rem;
  color: var(--gold-primary);
  border-bottom: 1px solid var(--border-color);
}

.product-info {
  padding: 1.25rem;
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  justify-content: space-between;
  gap: 1rem;
}

.product-title {
  font-size: 1.1rem;
  font-weight: 600;
}

.product-meta {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.product-price {
  font-size: 1.25rem;
  font-weight: 700;
  color: var(--gold-primary);
}

/* ==========================================
   ABOUT US SECTION (FLEXBOX)
   ========================================== */
.about-container {
  display: flex; /* FLEXBOX */
  align-items: center;
  gap: 3rem;
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  border-radius: 16px;
  padding: 3rem;
}

.about-text {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 1.25rem;
}

.about-stats {
  display: flex; /* FLEXBOX */
  gap: 2rem;
  margin-top: 1rem;
}

.stat-box {
  display: flex;
  flex-direction: column;
}

.stat-number {
  font-size: 2rem;
  font-weight: 800;
  color: var(--gold-primary);
  font-family: 'Cinzel', serif;
}

.stat-label {
  font-size: 0.85rem;
  color: var(--text-muted);
}

.about-visual {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 8rem;
  color: rgba(212, 175, 55, 0.2);
}

/* ==========================================
   CONTACT & USER ACCOUNT SECTIONS (FLEXBOX)
   ========================================== */
.form-flex-container {
  display: flex; /* FLEXBOX */
  gap: 2.5rem;
  flex-wrap: wrap;
}

.form-card {
  flex: 1;
  min-width: 320px;
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  border-radius: 12px;
  padding: 2.5rem;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.form-group label {
  font-size: 0.9rem;
  color: var(--text-muted);
}

.form-group input,
.form-group textarea {
  background: var(--bg-accent);
  border: 1px solid var(--border-color);
  border-radius: 6px;
  padding: 0.8rem 1rem;
  color: var(--text-main);
  font-family: inherit;
  outline: none;
  transition: var(--transition);
}

.form-group input:focus,
.form-group textarea:focus {
  border-color: var(--gold-primary);
}

/* ==========================================
   FOOTER (FLEXBOX MULTI-COLUMN)
   ========================================== */
.footer {
  background: #080a0e;
  border-top: 1px solid var(--border-color);
  padding: 4rem 1.5rem 2rem;
  margin-top: 4rem;
}

.footer-container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex; /* FLEXBOX */
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 2.5rem;
  margin-bottom: 3rem;
}

.footer-col {
  flex: 1;
  min-width: 220px;
  display: flex;
  flex-direction: column;
  gap: 1.25rem;
}

.footer-col h4 {
  color: var(--gold-primary);
  font-size: 1.1rem;
}

.footer-links {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
}

.footer-links a {
  color: var(--text-muted);
  font-size: 0.9rem;
}

.footer-links a:hover {
  color: var(--gold-primary);
}

.social-links {
  display: flex; /* FLEXBOX */
  gap: 1rem;
}

.social-btn {
  width: 38px;
  height: 38px;
  border-radius: 50%;
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--text-muted);
  transition: var(--transition);
}

.social-btn:hover {
  border-color: var(--gold-primary);
  color: var(--gold-primary);
  transform: translateY(-3px);
}

.footer-bottom {
  max-width: 1200px;
  margin: 0 auto;
  padding-top: 2rem;
  border-top: 1px solid rgba(255, 255, 255, 0.05);
  display: flex; /* FLEXBOX */
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 1rem;
  font-size: 0.85rem;
  color: var(--text-muted);
}

/* ==========================================
   CART SIDE-DRAWER STYLES
   ========================================== */
.cart-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(4px);
  z-index: 1001;
  opacity: 0;
  visibility: hidden;
  transition: all 0.3s ease;
}

.cart-overlay.active {
  opacity: 1;
  visibility: visible;
}

.cart-drawer {
  position: fixed;
  top: 0;
  right: -380px;
  width: 360px;
  max-width: 90%;
  height: 100vh;
  background: var(--bg-card);
  border-left: 1px solid var(--border-color);
  z-index: 1002;
  display: flex;
  flex-direction: column;
  transition: right 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  box-shadow: -10px 0 30px rgba(0, 0, 0, 0.5);
}

.cart-drawer.active {
  right: 0;
}

.cart-header {
  padding: 1.5rem;
  border-bottom: 1px solid var(--border-color);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.cart-header h3 {
  color: var(--gold-primary);
  font-size: 1.2rem;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.close-cart-btn {
  background: none;
  border: none;
  color: var(--text-muted);
  font-size: 1.8rem;
  cursor: pointer;
}

.close-cart-btn:hover {
  color: var(--gold-primary);
}

.cart-body {
  padding: 1.5rem;
  flex: 1;
  overflow-y: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.cart-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: var(--bg-accent);
  padding: 0.85rem 1rem;
  border-radius: 8px;
  border: 1px solid var(--border-color);
}

.cart-item-title {
  font-weight: 600;
  font-size: 0.95rem;
}

.cart-item-price {
  color: var(--gold-primary);
  font-size: 0.85rem;
  font-weight: 700;
}

.cart-item-qty {
  color: var(--text-muted);
  font-size: 0.85rem;
}

.cart-footer {
  padding: 1.5rem;
  border-top: 1px solid var(--border-color);
  display: flex;
  flex-direction: column;
  gap: 1rem;
  background: var(--bg-main);
}

.cart-total {
  display: flex;
  justify-content: space-between;
  font-size: 1.1rem;
  font-weight: 700;
  color: var(--text-main);
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .hero {
    flex-direction: column;
    text-align: center;
  }
  .hero-content {
    align-items: center;
  }
  .about-container {
    flex-direction: column;
  }
  .nav-links {
    display: none;
  }
}

```


## OUTPUT

![alt text](<Screenshot 2026-10-31 115942.png>) 
![alt text](<Screenshot 2026-10-31 115958.png>) 
![alt text](<Screenshot 2026-10-31 120125.png>)
![alt text](<Screenshot 2026-10-31 120138.png>)



## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
