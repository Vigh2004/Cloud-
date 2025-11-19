<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Personal Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav>
        <div class="nav-container">
            <h1>My Website</h1>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <section id="home" class="hero">
        <div class="container">
            <h2>Welcome to My Simple Website</h2>
            <p>A clean, responsive site hosted on the cloud</p>
        </div>
    </section>

    <section id="about" class="about">
        <div class="container">
            <h2>About Me</h2>
            <p>This is a simple website built with HTML and CSS, deployed on GitHub Pages. It's fast, free, and easy to maintain!</p>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2>Contact</h2>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" rows="5" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 My Website. All rights reserved.</p>
    </footer>
</body>
</html>


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
}

.container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 20px;
}

nav {
    background: #333;
    color: white;
    padding: 1rem 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 20px;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-left: 2rem;
}

nav ul li a {
    color: white;
    text-decoration: none;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: #4CAF50;
}

.hero {
    background: linear-gradient(to right, #4CAF50, #45a049);
    color: white;
    padding: 150px 20px 100px;
    text-align: center;
}

.hero h2 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.about, .contact {
    padding: 80px 20px;
    text-align: center;
}

.about {
    background: #f4f4f4;
}

.about h2, .contact h2 {
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
}

.contact form {
    max-width: 600px;
    margin: 0 auto;
}

.contact input, .contact textarea {
    width: 100%;
    padding: 12px;
    margin-bottom: 15px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.contact button {
    background: #4CAF50;
    color: white;
    padding: 12px 30px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    transition: background 0.3s;
}

.contact button:hover {
    background: #45a049;
}

footer {
    background: #333;
    color: white;
    text-align: center;
    padding: 20px;
}

@media (max-width: 768px) {
    .nav-container {
        flex-direction: column;
    }
    
    nav ul {
        margin-top: 10px;
    }
    
    nav ul li {
        margin: 0 10px;
    }
    
    .hero h2 {
        font-size: 2rem;
    }
}
