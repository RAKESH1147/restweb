# Ex.07 Restaurant Website
## Date:30/04/2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
home.html
```
html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Irani Restaurant</title>
  <style>
    :root {
      --dark-brown: #4e342e;
      --medium-brown: #795548;
      --sandal: #f1e1c1;
      --text-light: #fff;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--sandal);
      color: var(--dark-brown);
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: var(--dark-brown);
      padding: 15px 30px;
      color: var(--text-light);
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .nav-links {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    .nav-links li a {
      color: var(--text-light);
      text-decoration: none;
      font-size: 1rem;
    }

    .nav-links li a:hover {
      color: var(--sandal);
    }

    .hero {
      position: relative;
      background: url('https://images.unsplash.com/photo-1625940849482-df57bd1637a0') no-repeat center center/cover;
      height: 90vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    .hero-overlay {
      background-color: rgba(0, 0, 0, 0.5);
      padding: 60px 20px;
      border-radius: 10px;
    }

    .hero h1 {
      font-size: 3rem;
    }

    .hero p {
      font-size: 1.2rem;
      margin-top: 15px;
    }

    .hero button {
      margin-top: 25px;
      padding: 12px 25px;
      font-size: 1rem;
      border: none;
      border-radius: 5px;
      background-color: var(--sandal);
      color: var(--dark-brown);
      cursor: pointer;
    }

    .hero button:hover {
      background-color: var(--dark-brown);
      color: white;
    }

    .section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: auto;
    }

    .features {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      gap: 30px;
      text-align: center;
    }

    .feature-box {
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      flex: 1 1 250px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }

    .feature-box img {
      width: 60px;
      margin-bottom: 10px;
    }

    .feature-box h3 {
      margin-bottom: 10px;
      color: var(--medium-brown);
    }

    .dishes {
      display: flex;
      flex-wrap: wrap;
      gap: 30px;
      justify-content: space-between;
    }

    .dish {
      background-color: white;
      flex: 1 1 300px;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }

    .dish img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .dish h4 {
      padding: 15px;
      text-align: center;
      color: var(--medium-brown);
    }

    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2rem;
      }

      .features, .dishes {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>

  <nav class="navbar">
    <div class="logo">Irani Restaurant</div>
    <ul class="nav-links">
      <li><a href="index.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <div class="hero-overlay">
      <h1>Welcome to Irani Restaurant</h1>
      <p>Authentic flavors, warm ambiance, and timeless tradition</p>
      <button onclick="location.href='menu.html'">Explore Menu</button>
    </div>
  </section>

  <!-- Why Choose Us Section -->
  <section class="section">
    <h2 style="text-align:center; margin-bottom:40px;">Why Choose Us</h2>
    <div class="features">
      <div class="feature-box">
        <img src="https://cdn-icons-png.flaticon.com/512/1046/1046784.png" alt="Fresh">
        <h3>Fresh Ingredients</h3>
        <p>Only the best, locally sourced spices and meats for genuine taste.</p>
      </div>
      <div class="feature-box">
        <img src="https://cdn-icons-png.flaticon.com/512/684/684908.png" alt="Tradition">
        <h3>Irani Tradition</h3>
        <p>Time-tested recipes passed down through generations.</p>
      </div>
      <div class="feature-box">
        <img src="https://cdn-icons-png.flaticon.com/512/3050/3050541.png" alt="Atmosphere">
        <h3>Cozy Ambience</h3>
        <p>Warm, welcoming space perfect for family and friends.</p>
      </div>
    </div>
  </section>

  <!-- Featured Dishes Section -->
  <section class="section">
    <h2 style="text-align:center; margin-bottom:40px;">Featured Dishes</h2>
    <div class="dishes">
      <div class="dish">
        <img src="mandi.jpg" alt="Chicken Mandi">
        <h4>Chicken Mandi</h4>
      </div>
      <div class="dish">
        <img src="meetha.png">
        <h4>Double Ka Meetha</h4>
      </div>
      <div class="dish">
        <img src="kebab.png">
        <h4>Mutton Seekh Kebab</h4>
      </div>
    </div>
  </section>

</body>
</html>
```
menu.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Menu - Irani Restaurant</title>
  <style>
    :root {
      --dark-brown: #4e342e;
      --medium-brown: #795548;
      --sandal: #f1e1c1;
      --text-light: #fff;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--sandal);
      color: var(--dark-brown);
      line-height: 1.6;
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: var(--dark-brown);
      padding: 15px 30px;
      color: var(--text-light);
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .nav-links {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    .nav-links li a {
      color: var(--text-light);
      text-decoration: none;
      font-size: 1rem;
      transition: color 0.3s;
    }

    .nav-links li a:hover {
      color: var(--sandal);
    }

    .menu-section {
      padding: 40px 20px;
      max-width: 800px;
      margin: auto;
    }

    .menu-section h2 {
      font-size: 2rem;
      border-bottom: 2px solid var(--medium-brown);
      padding-bottom: 10px;
      margin-bottom: 20px;
    }

    .menu-item {
      margin-bottom: 15px;
    }

    .menu-item span {
      float: right;
      color: var(--medium-brown);
    }

    hr {
      border: none;
      border-top: 1px solid #ccc;
      margin: 40px 0;
    }

    @media (max-width: 600px) {
      .nav-links {
        flex-direction: column;
        gap: 10px;
      }

      .menu-section {
        padding: 20px;
      }
    }
  </style>
</head>
<body>

  <nav class="navbar">
    <div class="logo">Irani Restaurant</div>
    <ul class="nav-links">
      <li><a href="index.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <div class="menu-section">
    <h2>Soups</h2>
    <div class="menu-item">Chicken Soup <span>₹120</span></div>
    <div class="menu-item">Mutton Paya Soup <span>₹150</span></div>
    <div class="menu-item">Veg Clear Soup <span>₹90</span></div>

    <hr>

    <h2>Starters</h2>
    <div class="menu-item">Chicken Tikka <span>₹220</span></div>
    <div class="menu-item">Mutton Seekh Kebab <span>₹250</span></div>
    <div class="menu-item">Paneer Tikka <span>₹180</span></div>

    <hr>

    <h2>Mandi</h2>
    <div class="menu-item">Chicken Mandi (Full) <span>₹450</span></div>
    <div class="menu-item">Mutton Mandi (Full) <span>₹550</span></div>
    <div class="menu-item">Mix Mandi (Chicken + Mutton) <span>₹600</span></div>

    <hr>

    <h2>Breads</h2>
    <div class="menu-item">Tandoori Roti <span>₹25</span></div>
    <div class="menu-item">Butter Naan <span>₹35</span></div>
    <div class="menu-item">Rumali Roti <span>₹20</span></div>

    <hr>

    <h2>Desserts</h2>
    <div class="menu-item">Double Ka Meetha <span>₹90</span></div>
    <div class="menu-item">Khubani Ka Meetha <span>₹100</span></div>
    <div class="menu-item">Phirni <span>₹80</span></div>
  </div>

</body>
</html>

```
contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Contact - Irani Restaurant</title>
  <style>
    :root {
      --dark-brown: #4e342e;
      --medium-brown: #795548;
      --sandal: #f1e1c1;
      --text-light: #fff;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--sandal);
      color: var(--dark-brown);
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: var(--dark-brown);
      padding: 15px 30px;
      color: var(--text-light);
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .nav-links {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    .nav-links li a {
      color: var(--text-light);
      text-decoration: none;
      font-size: 1rem;
    }

    .nav-links li a:hover {
      color: var(--sandal);
    }

    .contact-section {
      max-width: 600px;
      margin: 60px auto;
      padding: 30px;
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    .contact-section h2 {
      margin-bottom: 20px;
      color: var(--medium-brown);
    }

    .contact-section p {
      margin-bottom: 15px;
    }

    .contact-section strong {
      color: var(--dark-brown);
    }

    @media (max-width: 600px) {
      .nav-links {
        flex-direction: column;
        gap: 10px;
      }

      .contact-section {
        margin: 30px 15px;
        padding: 20px;
      }
    }
  </style>
</head>
<body>

  <nav class="navbar">
    <div class="logo">Irani Restaurant</div>
    <ul class="nav-links">
      <li><a href="index.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>

  <div class="contact-section">
    <h2>Contact Us</h2>
    <p><strong>Address:</strong> 123 Irani Lane, Hyderabad, India</p>
    <p><strong>Phone:</strong> +91 98765 43210</p>
    <p><strong>Email:</strong> contact@iranirestaurant.com</p>
    <p>We’re open from <strong>12:00 PM to 11:00 PM</strong> every day.</p>
  </div>

</body>
</html>
```

## OUTPUT:
![alt text](<rakesh/restapp/static/Screenshot 2025-04-30 230446.png>)
![alt text](<rakesh/restapp/static/Screenshot 2025-04-30 230519.png>)
![alt text](<rakesh/restapp/static/Screenshot 2025-04-30 230542.png>)
![alt text](<rakesh/restapp/static/Screenshot 2025-04-30 230606.png>)
![alt text](<rakesh/restapp/static/Screenshot 2025-04-30 230648.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
