<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bake Sale Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to Our Bake Sale!</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#newsletter">Newsletter</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h2>Delicious Baked Goods</h2>
        <p>Browse our selection of fresh, homemade baked goods. Perfect for any occasion!</p>
    </section>

    <section id="products">
        <h2>Our Products</h2>
        <div class="product-list">
            <!-- Example Product -->
            <div class="product-item">
                <img src="cake.jpg" alt="Chocolate Cake">
                <h3>Chocolate Cake</h3>
                <p>$20.00</p>
                <button class="add-to-cart" data-product-id="1">Add to Cart</button>
            </div>
            <!-- Add more products here -->
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contact-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>

            <button type="submit">Send</button>
        </form>
    </section>

    <section id="newsletter">
        <h2>Sign Up for Our Newsletter</h2>
        <form id="newsletter-form">
            <label for="newsletter-email">Email:</label>
            <input type="email" id="newsletter-email" name="newsletter-email" required>
            <button type="submit">Subscribe</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Bake Sale. All rights reserved.</p>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>

/* styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #ffcc99;
    padding: 20px;
    text-align: center;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    text-decoration: none;
    color: #333;
}

h1, h2 {
    color: #d2691e;
}

.product-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

.product-item {
    margin: 20px;
    text-align: center;
}

.product-item img {
    max-width: 100%;
    height: auto;
}

#contact-form, #newsletter-form {
    display: flex;
    flex-direction: column;
    max-width: 400px;
    margin: 0 auto;
}

#contact-form label, #newsletter-form label {
    margin-top: 10px;
}

#contact-form input, #newsletter-form input, 
#contact-form textarea, #newsletter-form button {
    margin-top: 5px;
    padding: 10px;
    font-size: 1em;
}

footer {
    background-color: #ffcc99;
    padding: 10px;
    text-align: center;
}
