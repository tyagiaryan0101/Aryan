<!DOCTYPE html>
<html>
<head>
    <title> Gym Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <div id="header">
        <h1>TYAGI FITNESS CENTRE</h1>
        <div>
            <a href="#home">Home</a> | 
            <a href="#programs">Programs</a> | 
            <a href="#contact">Contact</a>
        </div>
    </div>

    <!-- Home Section -->
    <div id="home" class="section">
        <h2>Welcome to Our Gym</h2>
        <p>Get fit, stay healthy, and build strength with us.</p>
        
        <!-- Gym Picture -->
        <img src="https://images.unsplash.com/photo-1534438327276-14e5300c3a48?auto=format&fit=crop&w=600&q=80" alt="Gym Interior" class="gym-img">
        
        <br><br>
        <button onclick="welcomeMessage()">Click Me</button>
    </div>

    <!-- Programs Section -->
    <div id="programs" class="section">
        <h2>Our Programs</h2>
        
        <!-- Program Pictures Grid -->
        <div class="image-gallery">
            <div class="img-container">
                <img src="https://images.unsplash.com/photo-1581009146145-b5ef050c2e1e?auto=format&fit=crop&w=300&q=80" alt="Weight Lifting">
                <p>Weight Lifting</p>
            </div>
            <div class="img-container">
                <img src="https://images.unsplash.com/photo-1518611012118-696072aa579a?auto=format&fit=crop&w=300&q=80" alt="Cardio">
                <p>Cardio & Running</p>
            </div>
            <div class="img-container">
                <img src="https://images.unsplash.com/photo-1545205597-3d9d02c29597?auto=format&fit=crop&w=300&q=80" alt="Yoga">
                <p>Yoga Class</p>
            </div>
        </div>
    </div>

    <!-- Contact Section -->
    <div id="contact" class="section">
        <h2>Contact Us</h2>
        <p>Email: tyagi@mygym.com</p>
        <p>Phone: 9315352970</p>
    </div>

    <script src="first.js"></script>
</body>
</html>





body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

#header {
    background-color: #333;
    color: white;
    padding: 15px;
    text-align: center;
}

#header a {
    color: white;
    text-decoration: none;
    margin: 0 10px;
}

.section {
    padding: 40px;
    margin: 20px;
    background-color: white;
    border-radius: 5px;
    text-align: center;
}

/* Image Styling */
.gym-img {
    width: 80%;
    max-width: 500px;
    height: auto;
    border-radius: 8px;
    margin-top: 15px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.image-gallery {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin-top: 20px;
}

.img-container img {
    width: 250px;
    height: 160px;
    object-fit: cover;
    border-radius: 6px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.img-container p {
    font-weight: bold;
    margin-top: 8px;
}

button {
    padding: 10px 20px;
    background-color: #ff4757;
    color: white;
    border: none;
    cursor: pointer;
    border-radius: 4px;
}

button:hover {
    background-color: #ff6b81;
}


function welcomeMessage() {
    alert("Welcome to our Gym! Let's start your fitness journey.");
}
