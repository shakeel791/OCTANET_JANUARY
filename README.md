# OCTANET_JANUARY
1. HTML Structure //
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Learn to Code with Us</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">
                <h1>Code Academy</h1>
            </div>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#courses">Courses</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h2>Unlock the Power of Coding</h2>
        <p>Start your coding journey today and build the future you desire.</p>
        <a href="#contact" class="cta-btn">Get Started</a>
    </section>

    <section id="about" class="about">
        <h2>Why Learn with Us?</h2>
        <p>Our interactive courses cater to beginners and experts alike. You will learn through projects, challenges, and hands-on experience.</p>
    </section>

    <section id="courses" class="courses">
        <h2>Our Courses</h2>
        <div class="course-list">
            <div class="course-item">
                <h3>Web Development</h3>
                <p>Learn HTML, CSS, JavaScript, and frameworks like React and Node.js.</p>
            </div>
            <div class="course-item">
                <h3>Python for Beginners</h3>
                <p>Start programming with Python and build real-world applications.</p>
            </div>
            <div class="course-item">
                <h3>Data Science</h3>
                <p>Learn how to analyze and visualize data using Python and libraries like Pandas.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <form id="contact-form">
            <label for="name">Name:</label>
            <input type="text" id="name" required placeholder="Your name">
            
            <label for="email">Email:</label>
            <input type="email" id="email" required placeholder="Your email">

            <label for="message">Message:</label>
            <textarea id="message" required placeholder="Write your message"></textarea>
            
            <button type="submit">Submit</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Code Academy. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

2. CSS Styles (styles.css)//
/* General styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
}

nav .logo h1 {
    margin-left: 20px;
    font-size: 1.8em;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: flex-end;
}

nav ul li {
    margin-right: 20px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-size: 1.1em;
}

/* Hero Section */
.hero {
    background: linear-gradient(to right, #0099ff, #66ccff);
    color: white;
    text-align: center;
    padding: 80px 20px;
}

.hero h2 {
    font-size: 3em;
    margin-bottom: 20px;
}

.hero p {
    font-size: 1.5em;
    margin-bottom: 20px;
}

.cta-btn {
    padding: 12px 30px;
    font-size: 1.2em;
    background-color: #ff5722;
    color: white;
    text-decoration: none;
    border-radius: 5px;
}

/* About Section */
.about {
    padding: 40px 20px;
    text-align: center;
    background-color: #fff;
}

.about h2 {
    font-size: 2.5em;
    margin-bottom: 20px;
}

/* Courses Section */
.courses {
    padding: 40px 20px;
    text-align: center;
    background-color: #f9f9f9;
}

.courses h2 {
    font-size: 2.5em;
    margin-bottom: 20px;
}

.course-list {
    display: flex;
    justify-content: center;
    gap: 30px;
}

.course-item {
    background-color: #fff;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 300px;
}

.course-item h3 {
    font-size: 1.8em;
    margin-bottom: 10px;
}

/* Contact Section */
.contact {
    padding: 40px 20px;
    text-align: center;
    background-color: #fff;
}

.contact h2 {
    font-size: 2.5em;
    margin-bottom: 20px;
}

form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

form input, form textarea {
    margin-bottom: 10px;
    padding: 10px;
    width: 100%;
    max-width: 400px;
    border: 1px solid #ddd;
    border-radius: 5px;
}

form button {
    background-color: #0099ff;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

/* Footer */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
    position: fixed;
    width: 100%;
    bottom: 0;
}

3. JavaScript for Form Validation (script.js) //
document.getElementById('contact-form').addEventListener('submit', function (event) {
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;

    if (!name || !email || !message) {
        event.preventDefault();
        alert('Please fill in all fields!');
    } else {
        alert('Thank you for your message!');
    }
});
