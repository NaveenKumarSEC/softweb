# Ex.07 Restuarant Website
## Date:13-11-2025

## AIM:
To develop a static Resturant website to display the menu and services provided by the resturant.

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Naveen's Restaurant - Home</title>
    <link rel="icon" href="logos.jpg">
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background: #fafafa;
            color: #333;
        }
        .navbar {
            background: #2c3e50;
            overflow: hidden;
            box-shadow: 0 3px 6px rgba(0,0,0,0.16);
        }
        .navbar a {
            float: left;
            color: #ecf0f1;
            text-align: center;
            padding: 18px 24px;
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
            transition: background 0.3s;
        }
        .navbar a:hover, .navbar a.active {
            background: #34495e;
            color: #1abc9c;
        }
        .hero {
            background: url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
            height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #fff;
            text-shadow: 1px 1px 4px #000;
            text-align: center;
            padding: 0 20px;
        }
        .hero h1 {
            font-size: 48px;
            margin: 0;
            font-weight: 900;
        }
        .container {
            max-width: 900px;
            margin: 40px auto;
            background: #fff;
            padding: 30px 40px;
            border-radius: 12px;
            box-shadow: 0 6px 18px rgba(0,0,0,0.07);
        }
        h2 {
            color: #2c3e50;
            margin-bottom: 20px;
            font-weight: 700;
            border-bottom: 3px solid #1abc9c;
            display: inline-block;
            padding-bottom: 6px;
        }
        
    </style>
</head>
<body>
    <div class="navbar">
        
        <a href="home.html" class="active">Home</a>
        <a href="menu.html">Menu</a>
        <a href="contact.html">Contact</a>
        <a href="feedback.html">Feedback</a>
    </div>

    <section class="hero">
        <div>
            <h1>Welcome to Naveen's Restaurant</h1>
            <h4>Enjoy the taste of authentic dishes prepared with love and passion.</h4>
        </div>
    </section>
    <div class="container">
        <h2>About Us</h2>
        <p class="lead">We serve the finest food made from the freshest ingredients to satisfy your taste buds.</p>
        </div>
    </div>
</body>
</html>

```

menu.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Chandru Restaurant</title>
    <link rel="icon" href="logos.jpg">
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background-image: url(bg.jpg);
            background-repeat: no-repeat;
            background-size: cover;
            color: #333;
        }
        .navbar {
            background: #2c3e50;
            overflow: hidden;
            box-shadow: 0 3px 6px rgba(0,0,0,0.16);
        }
        .navbar a {
            float: left;
            color: #ecf0f1;
            text-align: center;
            padding: 18px 24px;
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
            transition: background 0.3s;
        }
        .navbar a:hover, .navbar a.active {
            background: #34495e;
            color: #1abc9c;
        }
        .container {
            max-width: 950px;
            margin: 40px auto;
            background: lightcyan;
            padding: 30px 40px;
            border-radius: 12px;
            box-shadow: 0 6px 18px rgba(0,0,0,0.07);
        }
        h2 {
            color: #2c3e50;
            margin-bottom: 30px;
            font-weight: 700;
            border-bottom: 3px solid #1abc9c;
            display: inline-block;
            padding-bottom: 6px;
        }
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        .menu-item {
            background: #ecf0f1;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
        }
        .menu-item:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }
        .menu-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-bottom: 3px solid #1abc9c;
        }
        .menu-content {
            padding: 15px 20px;
            text-align: center;
        }
        .menu-content h3 {
            color: #16a085;
            margin: 15px 0 10px;
            font-weight: 700;
            font-size: 20px;
        }
        .menu-content p {
            font-size: 16px;
            color: #555;
            margin: 0;
            font-weight: 600;
        }
        
    </style>
</head>
<body>
    <div class="navbar">
        <a href="home.html">Home</a>
        <a href="menu.html" class="active">Menu</a>
        <a href="contact.html">Contact</a>
        <a href="feedback.html">Feedback</a>
    </div>

    <div class="container">
        <h2>Menu</h2>
        <div class="menu-grid">
            <div class="menu-item">
                <img src="pizza.jpeg" alt="Margherita Pizza" />
                <div class="menu-content">
                    <h3>Margherita Pizza</h3>
                    <p>₹250</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Grilled Chicken Burger.jpeg" alt="Grilled Chicken Burger" />
                <div class="menu-content">
                    <h3>Grilled Chicken Burger</h3>
                    <p>₹180</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Pasta Alfredo.jpeg" alt="Pasta Alfredo" />
                <div class="menu-content">
                    <h3>Pasta Alfredo</h3>
                    <p>₹220</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Veggie Burger.jpeg" alt="Veggie Burger" />
                <div class="menu-content">
                    <h3>Veggie Burger</h3>
                    <p>₹150</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Classic Caesar Salad.jpeg" alt="Classic Caesar Salad" />
                <div class="menu-content">
                    <h3>Classic Caesar Salad</h3>
                    <p>₹120</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Chocolate Lava Cake.jpeg" alt="Chocolate Lava Cake" />
                <div class="menu-content">
                    <h3>Chocolate Lava Cake</h3>
                    <p>₹90</p>
                </div>
            </div>
        </div>
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
    <title>Chandru Restaurant</title>
    <link rel="icon" href="logos.jpg">
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            color: #333;
        }
        .navbar {
            background: #2c3e50;
            overflow: hidden;
            box-shadow: 0 3px 6px rgba(0,0,0,0.16);
        }
        .navbar a {
            float: left;
            color: #ecf0f1;
            text-align: center;
            padding: 18px 24px;
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
            transition: background 0.3s;
        }
        .navbar a:hover, .navbar a.active {
            background: #34495e;
            color: #1abc9c;
        }
        .container {
            max-width: 900px;
            margin: 40px auto 60px;
            background: whitesmoke;
            padding: 30px 40px;
            border-radius: 12px;
            box-shadow: 0 6px 18px rgba(0,0,0,0.07);
        }
        h2 {
            color: #2c3e50;
            margin-bottom: 25px;
            font-weight: 700;
            border-bottom: 3px solid #1abc9c;
            display: inline-block;
            padding-bottom: 6px;
        }
        .contact-details, .hours, .map-section {
            margin-bottom: 30px;
        }
        .contact-details p, .hours p {
            font-size: 17px;
            line-height: 1.6;
            color: teal;
            margin: 10px 0;
        }
        strong {
            color: black;
        }
        
    </style>
</head>
<body>
    <div class="navbar">
        <a href="home.html">Home</a>
        <a href="menu.html">Menu</a>
        <a href="contact.html" class="active">Contact</a>
        <a href="feedback.html">Feedback</a>
    </div>

    <div class="container">
        <h2>Contact Us</h2>

        <div class="contact-details">
            <p><strong>Email:</strong> naveenkumar11207@gmail.com</p>
            <p><strong>Phone:</strong> +91 7094161443</p>
            <p><strong>Address:</strong> 143 Main Road, Chennai, Tamil Nadu </p>
        </div>

        <div class="hours">
            <h2>Opening Hours</h2>
            <p><strong>Monday - Friday:</strong> 10:00 AM - 10:00 PM</p>
            <p><strong>Saturday - Sunday:</strong> 9:00 AM - 11:00 PM</p>
        </div>
    </div>
</body>
</html>

```

feedback.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Chandru Restaurant</title>
    <link rel="icon" href="logos.jpg">
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background: #fafafa;
            color: #333;
        }
        .navbar {
            background: #2c3e50;
            overflow: hidden;
            box-shadow: 0 3px 6px rgba(0,0,0,0.16);
        }
        .navbar a {
            float: left;
            color: #ecf0f1;
            text-align: center;
            padding: 18px 24px;
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
            transition: background 0.3s;
        }
        .navbar a:hover, .navbar a.active {
            background: #34495e;
            color: #1abc9c;
        }
        .container {
            max-width: 700px;
            margin: 40px auto;
            background: whitesmoke;
            padding: 30px 40px;
            border-radius: 12px;
            box-shadow: 0 6px 18px rgba(0,0,0,0.07);
        }
        h2 {
            color: #2c3e50;
            margin-bottom: 25px;
            font-weight: 700;
            border-bottom: 3px solid #1abc9c;
            display: inline-block;
            padding-bottom: 6px;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin: 15px 0 6px;
            font-weight: 600;
            color: #555;
        }
        input[type="text"],
        input[type="email"],
        select,
        textarea {
            padding: 10px 12px;
            border-radius: 6px;
            border: 1px solid #ccc;
            font-size: 16px;
            resize: vertical;
            font-family: inherit;
            transition: border-color 0.3s;
        }
        input[type="text"]:focus,
        input[type="email"]:focus,
        select:focus,
        textarea:focus {
            border-color: #1abc9c;
            outline: none;
            box-shadow: 0 0 4px #1abc9c;
        }
        textarea {
            min-height: 100px;
        }
        button {
            margin-top: 25px;
            background-color: #1abc9c;
            color: white;
            border: none;
            padding: 14px;
            font-size: 18px;
            font-weight: 700;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #16a085;
        }
        
    </style>
</head>
<body>
    <div class="navbar">
        <a href="home.html">Home</a>
        <a href="menu.html">Menu</a>
        <a href="contact.html">Contact</a>
        <a href="feedback.html" class="active">Feedback</a>
    </div>

    <div class="container">
        <h2>Feedback</h2>
        <form action="#" method="post">
            <label for="name">Name *</label>
            <input type="text" id="name" name="name" placeholder="Your full name" required />

            <label for="email">Email *</label>
            <input type="email" id="email" name="email" placeholder="Your email address" required />

            <label for="rating">How would you rate us? *</label>
            <select id="rating" name="rating" required>
                <option value="" disabled selected>Select rating</option>
                <option value="5">Excellent - 5</option>
                <option value="4">Very Good - 4</option>
                <option value="3">Good - 3</option>
                <option value="2">Fair - 2</option>
                <option value="1">Poor - 1</option>
            </select>

            <label for="comments">Comments</label>
            <textarea id="comments" name="comments" placeholder="Your valuable feedback or suggestions"></textarea>

            <button type="submit">Submit Feedback</button>
        </form>
    </div>
</body>
</html>

```

## OUTPUT:

![alt text](<Screenshot 2025-11-13 220105.png>)

![alt text](<Screenshot 2025-11-13 220157.png>)

![alt text](<Screenshot 2025-11-13 220227.png>)

![alt text](<Screenshot 2025-11-13 220252.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
