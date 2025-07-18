
## 2. Kodi i Plotë HTML (`index.html`)

```html
<!DOCTYPE html>
<html lang="sq">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Nordic Import AL - Specializuar në importin e produkteve premium për fëmijë nga LIBERO dhe marka të tjera europiane">
    <meta name="keywords" content="produkte për fëmijë, pelena libero, import nga europa, kremra për fëmijë">
    <title>NORDIC IMPORT AL - Produkte Premium për Fëmijë</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700&family=Roboto:wght@300;400;500&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="logo">
                <img src="images/logo.png" alt="Nordic Import AL Logo">
                <h1>NORDIC IMPORT AL</h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#home">Ballina</a></li>
                    <li><a href="#products">Produktet</a></li>
                    <li><a href="#about">Rreth Nesh</a></li>
                    <li><a href="#contact">Kontakt</a></li>
                    <li class="cart-icon"><a href="#cart"><i class="fas fa-shopping-cart"></i> <span id="cart-count">0</span></a></li>
                </ul>
            </nav>
            <div class="mobile-menu">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h2>Produkte Premium për Fëmijë nga LIBERO</h2>
            <p>Kremra, pelena dhe ushqime të gatshme me cilësi europiane</p>
            <div class="hero-buttons">
                <a href="#products" class="btn">Shiko Produktet</a>
                <a href="https://wa.me/355XXXXXXXX" class="btn whatsapp-btn"><i class="fab fa-whatsapp"></i> Na kontaktoni</a>
            </div>
        </div>
    </section>

    <!-- Produktet -->
    <section id="products" class="products">
        <div class="container">
            <h2 class="section-title">Produktet Tona</h2>
            <div class="product-filters">
                <button class="filter-btn active" data-filter="all">Të gjitha</button>
                <button class="filter-btn" data-filter="kremra">Kremra</button>
                <button class="filter-btn" data-filter="pelena">Pelena</button>
                <button class="filter-btn" data-filter="ushqim">Ushqim</button>
            </div>
            <div class="product-grid" id="product-container">
                <!-- Produktet do të ngarkohen dinamikisht nga script.js -->
            </div>
        </div>
    </section>

    <!-- Rreth Nesh -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">Rreth Nesh</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Nordic Import AL është specializuar në importin e produkteve premium për fëmijë nga Evropa. Ne ofrojmë vetëm produkte me cilësi të lartë, të testuara dhe të certifikuara sipas standardeve europiane.</p>
                    <p>Që nga viti 2015, ne kemi sjellë në tregun shqiptar produktet më të mira nga markat më të njohura në Evropë.</p>
                    <ul class="about-features">
                        <li><i class="fas fa-check"></i> Produkte 100% origjinale</li>
                        <li><i class="fas fa-check"></i> Certifikime europiane</li>
                        <li><i class="fas fa-check"></i> Dorëzim i shpejtë</li>
                    </ul>
                </div>
                <div class="about-image">
                    <img src="images/about-image.jpg" alt="Rreth Nordic Import AL" loading="lazy">
                </div>
            </div>
        </div>
    </section>

    <!-- Kontakt -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Na Kontaktoni</h2>
            <div class="contact-grid">
                <div class="contact-info">
                    <h3>Informacion Kontakti</h3>
                    <p><i class="fas fa-envelope"></i> nordicimportal@gmail.com</p>
                    <p><i class="fas fa-phone"></i> +355 XX XXX XXXX</p>
                    <p><i class="fas fa-map-marker-alt"></i> Tirana, Albania</p>
                    
                    <h3 class="social-title">Rrjetet Sociale</h3>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="https://wa.me/355XXXXXXXX"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                <div class="contact-form">
                    <form id="contactForm">
                        <div class="form-group">
                            <input type="text" id="name" placeholder="Emri Juaj*" required>
                        </div>
                        <div class="form-group">
                            <input type="email" id="email" placeholder="Email Juaj*" required>
                        </div>
                        <div class="form-group">
                            <input type="tel" id="phone" placeholder="Telefoni">
                        </div>
                        <div class="form-group">
                            <textarea id="message" placeholder="Mesazhi Juaj*" required></textarea>
                        </div>
                        <button type="submit" class="btn">Dërgo Mesazhin</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Shporta Modal -->
    <div id="cart-modal" class="modal">
        <div class="modal-content">
            <span class="close-modal">&times;</span>
            <h2>Shporta Juaj</h2>
            <div id="cart-items" class="cart-items">
                <!-- Produktet në shportë do të shfaqen këtu -->
                <p class="empty-cart">Shporta juaj është bosh</p>
            </div>
            <div class="cart-total">
                <p>Totali: <span id="cart-total">0</span> Lekë</p>
                <button id="checkout-btn" class="btn">Blej Tani</button>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-col">
                    <h3>Nordic Import AL</h3>
                    <p>Specialist në produkte për fëmijë me cilësi europiane</p>
                </div>
                <div class="footer-col">
                    <h3>Linqe të Shpejta</h3>
                    <ul>
                        <li><a href="#home">Ballina</a></li>
                        <li><a href="#products">Produktet</a></li>
                        <li><a href="#about">Rreth Nesh</a></li>
                        <li><a href="#contact">Kontakt</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Orari i Punës</h3>
                    <p>E Hënë - E Premte: 08:00 - 17:00</p>
                    <p>E Shtunë: 09:00 - 14:00</p>
                    <p>E Dielë: Mbyllur</p>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2023 NORDIC IMPORT AL. Të gjitha të drejtat e rezervuara.</p>
            </div>
        </div>
    </footer>

    <!-- Back to Top Button -->
    <a href="#home" class="back-to-top"><i class="fas fa-arrow-up"></i></a>

    <script src="script.js"></script>
</body>
</html>
```

## 3. Kodi i Plotë CSS (`style.css`)

```css
/* ============ VARIABLA ============ */
:root {
    --primary-color: #003366;
    --primary-dark: #002244;
    --primary-light: #3a6ea5;
    --secondary-color: #ff6b6b;
    --accent-color: #ff9f1c;
    --light-color: #f9f9f9;
    --dark-color: #333;
    --text-color: #444;
    --gray-color: #e0e0e0;
    --border-radius: 8px;
    --box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    --transition: all 0.3s ease;
}

/* ============ RESET & BASE STYLES ============ */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Open Sans', sans-serif;
    line-height: 1.6;
    color: var(--text-color);
    background: var(--light-color);
    overflow-x: hidden;
}

h1, h2, h3, h4 {
    font-family: 'Roboto', sans-serif;
    font-weight: 700;
    color: var(--dark-color);
}

a {
    text-decoration: none;
    color: inherit;
}

ul {
    list-style: none;
}

img {
    max-width: 100%;
    height: auto;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 15px;
}

.btn {
    display: inline-block;
    background: var(--secondary-color);
    color: white;
    padding: 12px 25px;
    border: none;
    border-radius: var(--border-radius);
    cursor: pointer;
    font-weight: 600;
    transition: var(--transition);
    text-align: center;
}

.btn:hover {
    background: #ff5252;
    transform: translateY(-3px);
    box-shadow: var(--box-shadow);
}

.whatsapp-btn {
    background: #25D366;
}

.whatsapp-btn:hover {
    background: #128C7E;
}

.section-title {
    text-align: center;
    margin-bottom: 3rem;
    font-size: 2.2rem;
    color: var(--primary-color);
    position: relative;
}

.section-title::after {
    content: '';
    display: block;
    width: 80px;
    height: 4px;
    background: var(--accent-color);
    margin: 1rem auto;
}

/* ============ HEADER ============ */
header {
    background: var(--primary-color);
    color: white;
    padding: 1rem 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    transition: var(--transition);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

header.scrolled {
    background: var(--primary-dark);
    padding: 0.5rem 0;
}

.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;
}

.logo img {
    height: 40px;
}

.logo h1 {
    font-size: 1.5rem;
    margin: 0;
    color: white;
}

nav ul {
    display: flex;
    gap: 2rem;
}

nav ul li a {
    font-weight: 600;
    transition: var(--transition);
    position: relative;
}

nav ul li a:hover {
    color: var(--secondary-color);
}

nav ul li a::after {
    content: '';
    position: absolute;
    width: 0;
    height: 2px;
    background: var(--secondary-color);
    bottom: -5px;
    left: 0;
    transition: var(--transition);
}

nav ul li a:hover::after {
    width: 100%;
}

.cart-icon {
    position: relative;
}

.cart-icon span {
    position: absolute;
    top: -10px;
    right: -10px;
    background: var(--secondary-color);
    color: white;
    border-radius: 50%;
    width: 20px;
    height: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.7rem;
    font-weight: bold;
}

.mobile-menu {
    display: none;
    font-size: 1.5rem;
    cursor: pointer;
}

/* ============ HERO SECTION ============ */
.hero {
    height: 100vh;
    min-height: 600px;
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('images/hero-bg.jpg') no-repeat center center/cover;
    color: white;
    display: flex;
    align-items: center;
    text-align: center;
    padding-top: 80px;
}

.hero-content {
    max-width: 800px;
    margin: 0 auto;
    padding: 2rem;
    animation: fadeIn 1s ease;
}

.hero h2 {
    font-size: 2.8rem;
    margin-bottom: 1.5rem;
    line-height: 1.2;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 2.5rem;
    opacity: 0.9;
}

.hero-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

/* ============ PRODUCTS SECTION ============ */
.products {
    padding: 5rem 0;
    background: white;
}

.product-filters {
    display: flex;
    justify-content: center;
    gap: 1rem;
    margin-bottom: 2rem;
    flex-wrap: wrap;
}

.filter-btn {
    padding: 0.5rem 1.5rem;
    border: 1px solid var(--gray-color);
    background: white;
    border-radius: 30px;
    cursor: pointer;
    transition: var(--transition);
}

.filter-btn.active, .filter-btn:hover {
    background: var(--primary-color);
    color: white;
    border-color: var(--primary-color);
}

.product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 2rem;
}

.product-card {
    background: white;
    border-radius: var(--border-radius);
    overflow: hidden;
    box-shadow: var(--box-shadow);
    transition: var(--transition);
    position: relative;
}

.product-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

.product-card img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    transition: var(--transition);
}

.product-card:hover img {
    transform: scale(1.05);
}

.product-info {
    padding: 1.5rem;
}

.product-card h3 {
    font-size: 1.2rem;
    margin-bottom: 0.5rem;
    color: var(--primary-color);
}

.product-card p {
    color: var(--text-color);
    margin-bottom: 1rem;
    font-size: 0.95rem;
}

.product-price {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 1rem;
}

.price {
    font-size: 1.2rem;
    font-weight: bold;
    color: var(--secondary-color);
}

.add-to-cart {
    background: var(--primary-color);
    color: white;
    border: none;
    padding: 0.5rem 1rem;
    border-radius: var(--border-radius);
    cursor: pointer;
    transition: var(--transition);
}

.add-to-cart:hover {
    background: var(--primary-dark);
}

/* ============ ABOUT SECTION ============ */
.about {
    padding: 5rem 0;
    background: var(--light-color);
}

.about-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
}

.about-text p {
    margin-bottom: 1.5rem;
    line-height: 1.8;
}

.about-features {
    margin: 2rem 0;
}

.about-features li {
    margin-bottom: 0.8rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
}

.about-features i {
    color: var(--accent-color);
}

.about-image {
    border-radius: var(--border-radius);
    overflow: hidden;
    box-shadow: var(--box-shadow);
}

.about-image img {
    width: 100%;
    height: auto;
    display: block;
    transition: var(--transition);
}

.about-image:hover img {
    transform: scale(1.05);
}

/* ============ CONTACT SECTION ============ */
.contact {
    padding: 5rem 0;
    background: white;
}

.contact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
}

.contact-info h3, .contact-form h3 {
    margin-bottom: 1.5rem;
    color: var(--primary-color);
    font-size: 1.5rem;
}

.contact-info p {
    margin-bottom: 1.5rem;
    display: flex;
    align-items: center;
    gap: 0.8rem;
}

.contact-info i {
    color: var(--accent-color);
    font-size: 1.2rem;
    width: 25px;
}

.social-title {
    margin-top: 2rem;
}

.social-links {
    display: flex;
    gap: 1rem;
    margin-top: 1rem;
}

.social-links a {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
    background: var(--primary-color);
    color: white;
    border-radius: 50%;
    transition: var(--transition);
}

.social-links a:hover {
    background: var(--secondary-color);
    transform: translateY(-3px);
}

.form-group {
    margin-bottom: 1.5rem;
}

.form-group input, .form-group textarea {
    width: 100%;
    padding: 0.8rem 1rem;
    border: 1px solid var(--gray-color);
    border-radius: var(--border-radius);
    font-family: inherit;
    transition: var(--transition);
}

.form-group input:focus, .form-group textarea:focus {
    outline: none;
    border-color: var(--primary-color);
    box-shadow: 0 0 0 3px rgba(0, 51, 102, 0.1);
}

.form-group textarea {
    height: 150px;
    resize: vertical;
}

/* ============ MODAL ============ */
.modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
    z-index: 2000;
    justify-content: center;
    align-items: center;
}

.modal-content {
    background: white;
    border-radius: var(--border-radius);
    width: 90%;
    max-width: 600px;
    max-height: 80vh;
    overflow-y: auto;
    padding: 2rem;
    position: relative;
    animation: modalFadeIn 0.3s ease;
}

@keyframes modalFadeIn {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
}

.close-modal {
    position: absolute;
    top: 15px;
    right: 15px;
    font-size: 1.5rem;
    cursor: pointer;
    color: var(--text-color);
    transition: var(--transition);
}

.close-modal:hover {
    color: var(--secondary-color);
}

.cart-items {
    margin: 1.5rem 0;
}

.cart-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 0;
    border-bottom: 1px solid var(--gray-color);
}

.cart-item img {
    width: 60px;
    height: 60px;
    object-fit: cover;
    border-radius: 4px;
}

.cart-item-info {
    flex: 1;
    padding: 0 1rem;
}

.cart-item-title {
    font-weight: 600;
    margin-bottom: 0.3rem;
}

.cart-item-price {
    color: var(--secondary-color);
    font-weight: bold;
}

.cart-item-remove {
    color: var(--text-color);
    cursor: pointer;
    transition: var(--transition);
}

.cart-item-remove:hover {
    color: var(--secondary-color);
}

.cart-total {
    text-align: right;
    font-size: 1.2rem;
    margin-top: 1.5rem;
    padding-top: 1rem;
    border-top: 2px solid var(--primary-color);
}

.cart-total span {
    color: var(--secondary-color);
    font-weight: bold;
}

.empty-cart {
    text-align: center;
    padding: 2rem;
    color: var(--text-color);
}

/* ============ FOOTER ============ */
footer {
    background: var(--primary-dark);
    color: white;
    padding: 4rem 0 0;
}

.footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin-bottom: 2rem;
}

.footer-col h3 {
    color: white;
    margin-bottom: 1.5rem;
    font-size: 1.3rem;
    position: relative;
    padding-bottom: 0.5rem;
}

.footer-col h3::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    width: 50px;
    height: 2px;
    background: var(--accent-color);
}

.footer-col p, .footer-col li {
    margin-bottom: 0.8rem;
    opacity: 0.8;
}

.footer-col a {
    transition: var(--transition);
}

.footer-col a:hover {
    color: var(--secondary-color);
}

.footer-bottom {
    text-align: center;
    padding: 1.5rem 0;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    font-size: 0.9rem;
    opacity: 0.7;
}

/* ============ BACK TO TOP ============ */
.back-to-top {
    position: fixed;
    bottom: 30px;
    right: 30px;
    width: 50px;
    height: 50px;
    background: var(--primary-color);
    color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.2rem;
    box-shadow: var(--box-shadow);
    opacity: 0;
    visibility: hidden;
    transition: var(--transition);
    z-index: 999;
}

.back-to-top.active {
    opacity: 1;
    visibility: visible;
}

.back-to-top:hover {
    background: var(--secondary-color);
}

/* ============ RESPONSIVE DESIGN ============ */
@media (max-width: 992px) {
    .about-content {
        grid-template-columns: 1fr;
    }
    
    .about-image {
        order: -1;
        max-width: 600px;
        margin: 0 auto;
    }
}

@media (max-width: 768px) {
    .hero h2 {
        font-size: 2.2rem;
    }
    
    .hero p {
        font-size: 1rem;
    }
    
    nav {
        position: fixed;
        top: 80px;
        left: -100%;
        width: 80%;
        height: calc(100vh - 80px);
        background: var(--primary-dark);
        flex-direction: column;
        padding: 2rem;
        transition: var(--transition);
    }
    
    nav.active {
        left: 0;
    }
    
    nav ul {
        flex-direction: column;
        gap: 1.5rem;
    }
    
    .mobile-menu {
        display: block;
    }
    
    .contact-grid {
        grid-template-columns: 1fr;
    }
    
    .footer-content {
        grid-template-columns: 1fr 1fr;
    }
}

@media (max-width: 576px) {
    .hero h2 {
        font-size: 1.8rem;
    }
    
    .hero-buttons {
        flex-direction: column;
    }
    
    .btn {
        width: 100%;
    }
    
    .product-grid {
        grid-template-columns: 1fr;
    }
    
    .footer-content {
        grid-template-columns: 1fr;
    }
    
    .modal-content {
        width: 95%;
        padding: 1.5rem;
    }
}
```

## 4. Kodi i Plotë JavaScript (`script.js`)

```javascript
// Document Ready
document.addEventListener('DOMContentLoaded', function() {
    // Mobile Menu Toggle
    const mobileMenuBtn = document.querySelector('.mobile-menu');
    const nav = document.querySelector('nav');
    
    mobileMenuBtn.addEventListener('click', function() {
        nav.classList.toggle('active');
        this.querySelector('i').classList.toggle('fa-times');
    });
    
    // Close mobile menu when clicking on a link
    document.querySelectorAll('nav a').forEach(link => {
        link.addEventListener('click', function() {
            if (window.innerWidth <= 768) {
                nav.classList.remove('active');
                mobileMenuBtn.querySelector('i').classList.remove('fa-times');
            }
        });
    });
    
    // Header Scroll Effect
    window.addEventListener('scroll', function() {
        const header = document.querySelector('header');
        const backToTop = document.querySelector('.back-to-top');
        
        if (window.scrollY > 100) {
            header.classList.add('scrolled');
            backToTop.classList.add('active');
        } else {
            header.classList.remove('scrolled');
            backToTop.classList.remove('active');
        }
    });
    
    // Product Filtering
    const filterBtns = document.querySelectorAll('.filter-btn');
    const productContainer = document.getElementById('product-container');
    
    // Sample product data (in a real app, this would come from an API or JSON file)
    const products = [
        {
            id: 1,
            name: 'Kremra Bebëlina',
            description: 'Për lëkurën e ndjeshme të foshnjave. Formulë pa parfum dhe paraben.',
            price: 2500,
            category: 'kremra',
            image: 'images/kremra-libero.jpg'
        },
        {
            id: 2,
            name: 'Pelena Libero',
            description: 'Pelena ultra-përthithëse pa alkool, me mbajtëse elastike.',
            price: 3200,
            category: 'pelena',
            image: 'images/pelena-libero.jpg'
        },
        {
            id: 3,
            name: 'Ushqim për Fëmijë',
            description: 'Ushqim organik për fëmijë mbi 6 muaj. Pa shtesa artificiale.',
            price: 1800,
            category: 'ushqim',
            image: 'images/baby-food.jpg'
        },
        {
            id: 4,
            name: 'Shampo për Fëmijë',
            description: 'Shampo me formulë delikate për fëmijë. Nuk i irriton sytë.',
            price: 2100,
            category: 'kremra',
            image: 'images/baby-shampoo.jpg'
        }
    ];
    
    // Display all products initially
    displayProducts(products);
    
    // Filter products
    filterBtns.forEach(btn => {
        btn.addEventListener('click', function() {
            // Remove active class from all buttons
            filterBtns.forEach(btn => btn.classList.remove('active'));
            
            // Add active class to clicked button
            this.classList.add('active');
            
            const filter = this.dataset.filter;
            
            if (filter === 'all') {
                displayProducts(products);
            } else {
                const filteredProducts = products.filter(product => product.category === filter);
                displayProducts(filteredProducts);
            }
        });
    });
    
    // Function to display products
    function displayProducts(productsToDisplay) {
        productContainer.innerHTML = '';
        
        if (productsToDisplay.length === 0) {
            productContainer.innerHTML = '<p class="no-products">Nuk u gjet asnjë produkt.</p>';
            return;
        }
        
        productsToDisplay.forEach(product => {
            const productCard = document.createElement('div');
            productCard.className = 'product-card';
            productCard.innerHTML = `
                <img src="${product.image}" alt="${product.name}" loading="lazy">
                <div class="product-info">
                    <h3>${product.name}</h3>
                    <p>${product.description}</p>
                    <div class="product-price">
                        <span class="price">${product.price} Lekë</span>
                        <button class="add-to-cart" data-id="${product.id}">Shto në Shportë</button>
                    </div>
                </div>
            `;
            
            productContainer.appendChild(productCard);
        });
        
        // Add event listeners to "Add to Cart" buttons
        document.querySelectorAll('.add-to-cart').forEach(btn => {
            btn.addEventListener('click', function() {
                const productId = parseInt(this.dataset.id);
                addToCart(productId);
            });
        });
    }
    
    // Cart functionality
    let cart = JSON.parse(localStorage.getItem('cart')) || [];
    const cartCount = document.getElementById('cart-count');
    const cartModal = document.getElementById('cart-modal');
    const closeModal = document.querySelector('.close-modal');
    const cartItemsContainer = document.getElementById('cart-items');
    const cartTotal = document.getElementById('cart-total');
    const checkoutBtn = document.getElementById('checkout-btn');
    
    // Update cart count
    updateCartCount();
    
    // Add to cart function
    function addToCart(productId) {
        const product = products.find(p => p.id === productId);
        
        if (!product) return;
        
        const existingItem = cart.find(item => item.id === productId);
        
        if (existingItem) {
            existingItem.quantity += 1;
        } else {
            cart.push({
                ...product,
                quantity: 1
            });
        }
        
        updateCart();
        showCartNotification(product.name);
    }
    
    // Update cart
    function updateCart() {
        localStorage.setItem('cart', JSON.stringify(cart));
        updateCartCount();
        renderCartItems();
    }
    
    // Update cart count
    function updateCartCount() {
        const totalItems = cart.reduce((total, item) => total + item.quantity, 0);
        cartCount.textContent = totalItems;
    }
    
    // Render cart items
    function renderCartItems() {
        if (cart.length === 0) {
            cartItemsContainer.innerHTML = '<p class="empty-cart">Shporta juaj është bosh</p>';
            cartTotal.textContent = '0';
            return;
        }
        
        cartItemsContainer.innerHTML = '';
        let total = 0;
        
        cart.forEach(item => {
            const cartItem = document.createElement('div');
            cartItem.className = 'cart-item';
            cartItem.innerHTML = `
                <img src="${item.image}" alt="${item.name}">
                <div class="cart-item-info">
                    <p class="cart-item-title">${item.name}</p>
                    <p class="cart-item-price">${item.price} Lekë x ${item.quantity}</p>
                </div>
                <i class="fas fa-times cart-item-remove" data-id="${item.id}"></i>
            `;
            
            cartItemsContainer.appendChild(cartItem);
            total += item.price * item.quantity;
        });
        
        cartTotal.textContent = total;
        
        // Add event listeners to remove buttons
        document.querySelectorAll('.cart-item-remove').forEach(btn => {
            btn.addEventListener('click', function() {
                const productId = parseInt(this.dataset.id);
                removeFromCart(productId);
            });
        });
    }
    
    // Remove from cart
    function removeFromCart(productId) {
        cart = cart.filter(item => item.id !== productId);
        updateCart();
    }
    
    // Show cart notification
    function showCartNotification(productName) {
        const notification = document.createElement('div');
        notification.className = 'notification';
        notification.innerHTML = `
            <p>${productName} u shtua në shportë!</p>
        `;
        
        document.body.appendChild(notification);
        
        setTimeout(() => {
            notification.classList.add('show');
        }, 10);
        
        setTimeout(() => {
            notification.classList.remove('show');
            setTimeout(() => {
                notification.remove();
            }, 300);
        }, 3000);
    }
    
    // Cart modal toggle
    document.querySelector('.cart-icon a').addEventListener('click', function(e) {
        e.preventDefault();
        cartModal.style.display = 'flex';
        renderCartItems();
    });
    
    closeModal.addEventListener('click', function() {
        cartModal.style.display = 'none';
    });
    
    window.addEventListener('click', function(e) {
        if (e.target === cartModal) {
            cartModal.style.display = 'none';
        }
    });
    
    // Checkout button
    checkoutBtn.addEventListener('click', function() {
        alert('Faleminderit 