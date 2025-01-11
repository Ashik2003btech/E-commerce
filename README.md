# Simple E-Commerce Website

This project is a **Simple E-Commerce Website** built using HTML and CSS. The website is simple, responsive, and designed for showcasing products. It includes a header, an embedded YouTube video, a product section, and a footer.

---

## Features

- **Navigation Bar**: Includes links to Home, Products, and Contact sections.
- **Embedded Video**: Displays a YouTube video.
- **Hero Section**: A welcoming section with a call-to-action button.
- **Product Section**: Displays three sample products with images, descriptions, and "Add to Cart" buttons.
- **Footer**: Contains contact information and copyright details.

---

## Project Structure


---

## HTML Code

Below is the complete `index.html` code used in this project:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple E-Commerce Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="logo">ShopEasy</div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="video-section">
        <iframe 
            width="100%" 
            height="400" 
            src="https://www.youtube.com/embed/s3-qGPGtE8s" 
            title="YouTube video player" 
            frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
            allowfullscreen>
        </iframe>
    </section>

    <section id="home" class="hero-section">
        <h1>Welcome to ShopEasy</h1>
        <p>Your one-stop shop for all your needs!</p>
        <a href="#products" class="btn">Shop Now</a>
    </section>

    <section id="products" class="products-section">
        <h2>Our Products</h2>
        <div class="product-container">
            <div class="product-card">
                <img src="image1" alt="Product 1">
                <h3>Kayme 7 Layers Heavy Duty Car Cover Waterproof All Weather, Universal Fit for Sedan Coupe Car (up to 165 inch), Such as Mazda Miata MX-5, Honda S2000.</h3>
                <p>$29.99</p>
                <button>Add to Cart</button>
            </div>
            <div class="product-card">
                <img src="image" alt="Product 2">
                <h3>Govee RGBIC LED Strip Lights, 65.6ft Smart LED Lights for Bedroom, Bluetooth LED Lights APP Control, DIY Multiple Colors on One Line </h3>
                <p>$39.99</p>
                <button>Add to Cart</button>
            </div>
            <div class="product-card">
                <img src="image2" alt="Product 3">
                <h3>Echo Spot Bundle: Includes Echo Spot (2024 Release) | Glacier White & Made for Amazon Stand with USB-C and USB-A Charging Ports | Glacier White</h3>
                <p>$99.99</p>
                <button>Add to Cart</button>
            </div>
        </div>
    </section>

    <footer id="contact">
        <p>Contact us at <a href="mailto:info@shopeasy.com">info@shopeasy.com</a></p>
        <p>&copy; 2025 ShopEasy. All rights reserved.</p>
    </footer>
</body>
</html>

/* General Styles */
body {
    margin: 0;
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background-color: #333;
    color: #fff;
}

header .logo {
    font-size: 1.5rem;
    font-weight: bold;
}

header nav ul {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
}

header nav ul li {
    margin-left: 1.5rem;
}

header nav ul li a {
    text-decoration: none;
    color: #fff;
    font-weight: bold;
    transition: color 0.3s;
}

header nav ul li a:hover {
    color: #ff9900;
}

/* Hero Section */
.hero-section {
    text-align: center;
    padding: 4rem 2rem;
    background: #f4f4f4;
}

.hero-section h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.hero-section p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.hero-section .btn {
    padding: 0.8rem 1.5rem;
    background-color: #333;
    color: #fff;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
    transition: background 0.3s;
}

.hero-section .btn:hover {
    background-color: #ff9900;
}

/* Products Section */
.products-section {
    padding: 2rem;
    background: #fff;
    text-align: center;
}

.products-section h2 {
    margin-bottom: 2rem;
    font-size: 2rem;
}

.product-container {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
}

.product-card {
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 1rem;
    max-width: 200px;
    text-align: center;
    background: #f9f9f9;
    transition: box-shadow 0.3s;
}

.product-card:hover {
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.product-card img {
    max-width: 100%;
    border-radius: 5px;
    margin-bottom: 1rem;
}

.product-card h3 {
    font-size: 1.2rem;
    margin-bottom: 0.5rem;
}

.product-card p {
    margin-bottom: 1rem;
    font-weight: bold;
}

.product-card button {
    padding: 0.5rem 1rem;
    background-color: #333;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background 0.3s;
}

.product-card button:hover {
    background-color: #ff9900;
}

/* Footer */
footer {
    text-align: center;
    padding: 1rem;
    background-color: #333;
    color: #fff;
    margin-top: 2rem;
}

footer a {
    color: #ff9900;
    text-decoration: none;
}


