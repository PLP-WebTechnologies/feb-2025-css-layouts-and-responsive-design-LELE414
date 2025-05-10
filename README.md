<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Travel Blog</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation Bar -->
    <nav class="navbar">
        <div class="logo">Travel Blog</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#destinations">Destinations</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Main Section (Grid Layout) -->
    <section id="home" class="main-section">
        <header>
            <h1>Welcome to the Travel Blog!</h1>
            <p>Your ultimate guide to exploring the world.</p>
        </header>

        <div class="grid-container">
            <article class="feature">
                <h2>Top Destinations</h2>
                <p>Explore the most popular travel destinations of the year.</p>
            </article>
            <article class="feature">
                <h2>Travel Tips</h2>
                <p>Learn the best tips for a smooth and exciting journey.</p>
            </article>
            <article class="feature">
 <h2>Adventure Stories</h2>
                <p>Read about amazing travel adventures from around the world.</p>
            </article>
        </div>
    </section>

    <!-- Footer Section -->
    <footer>
        <div class="footer-content">
            <p>&copy; 2025 Travel Blog | All Rights Reserved</p>
        </div>
    </footer>

</body>
</html>

/* Basic Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #333;
    color: white;
    padding: 1rem;
}

nav .logo {
    font-size: 1.5rem;
}

nav .nav-links {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
}

nav .nav-links li {
    margin-left: 20px;
}

nav .nav-links a {
    color: white;
    text-decoration: none;
    font-size: 1rem;
}

.main-section {
    text-align: center;
    padding: 2rem;
    background-color: #fff;
    color: #333;
}

header h1 {
    font-size: 2.5rem;
}

header p {
    font-size: 1.2rem;
}

.grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    margin-top: 2rem;
}

.feature {
    background-color: #eee;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.feature h2 {
    font-size: 1.8rem;
    margin-bottom: 1rem;
}

footer {
    background-color: #333;
    color: white;
    padding: 1rem;
    text-align: center;
}
footer .footer-content p {
    margin: 0;
}

/* Media Queries for Responsiveness */
@media (max-width: 1024px) {
    .grid-container {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 768px) {
    .grid-container {
        grid-template-columns: 1fr;
    }

    nav {
        flex-direction: column;
        text-align: center;
    }

    nav .nav-links {
        flex-direction: column;
        margin-top: 1rem;
    }

    nav .nav-links li {
        margin-bottom: 10px;
    }

    header h1 {
        font-size: 2rem;
    }
}

@media (max-width: 480px) {
    .feature {
        padding: 1rem;
    }

    header h1 {
        font-size: 1.5rem;
    }
 header p {
        font-size: 1rem;
    }
}
