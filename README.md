# Ex.07 Restaurant Website
## Date:07/10/2025
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
~~~
contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
            background-color: #f4f4f4;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #007BFF;
            color: #ffffff;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            height: 80px;
        }

        header nav a {
            padding: 10px 15px;
            text-decoration: none;
            color: #ffffff;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .contact-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 40px 20px;
            background: #ffffff;
            gap: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            margin: 20px;
        }

        .contact-details, .contact-form {
            flex: 1;
            max-width: 500px;
            margin: 10px;
            background: #f9f9f9;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .contact-details h2, .contact-form h2 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: #333;
            text-align: center;
        }

        .contact-details p {
            margin: 10px 0;
            font-size: 1rem;
            color: #555;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
            transition: border-color 0.3s ease;
        }

        .contact-form input:focus, .contact-form textarea:focus {
            border-color: #007BFF;
            outline: none;
        }

        .contact-form textarea {
            height: 100px;
        }

        .contact-form button {
            width: 100%;
            padding: 12px;
            background: #ff5722;
            color: white;
            font-size: 1.1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .contact-form button:hover {
            background: #e64a19;
        }

        footer {
            background: #007BFF;
            color: #ffffff;
            text-align: center;
            padding: 10px 0;
            margin-top: 20px;
        }

        @media (max-width: 768px) {
            .contact-details, .contact-form {
                max-width: 100%;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>AKSHUU</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="owners.html" class="active">Owner</a>
        </nav>
    </header>

    <section class="contact-section">
        <div class="contact-details">
            <h2>Get in Touch</h2>
            <p><strong>Phone:</strong> +91 8072215767</p>
            <p><strong>Email:</strong> akshuuuzii@gmail.com</p>
        </div>

        <div class="contact-form">
            <h2>Send Message</h2>
            <form action="/submit-contact" method="POST">
                <label for="name">Name</label>
                <input type="text" id="name" name=" name" placeholder="Enter Your Name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" placeholder="Enter Your Email" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" placeholder="Your Message" required></textarea>

                <button type="submit">Submit</button>
            </form>
        </div>
    </section>

    <footer>
        <p>Designed by: Sheik udhuman (25015367)</p>
    </footer>

</body>
</html>

home.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            height: 80px;
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .banner {
            background-size: cover;
            margin: 1% 2%;
            border-radius: 37px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 30px 20px;
            background: rgb(67, 69, 71);
            color: white;
            height: 250px;
            text-align: center;
        }

        .banner-content {
            max-width: 50%;
        }

        .banner-content h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .banner-content p {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }

        footer {
            background: white;
            color: rgb(0, 0, 0);
            text-align: center;
            padding: 10px 0;
            margin-top: 100px;
            font-size: larger;
        }

        @media (max-width: 768px) {
            .banner {
                flex-direction: column;
                height: auto;
                text-align: center;
            }

            .banner-content {
                max-width: 100%;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>AKS FOODIE HUB</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="owners.html" class="active">Owner</a>
        </nav>
    </header>
    <div class="logo">
        <center><img src="aksuzii.jpg" height="350px" width="350px"></center>
    </div>
    <div class="banner">
        <div class="banner-content">
            <h1>Welcome To "akshuu grand food park"</h1>
            <p>Where every flavor tells a story.</p>
        </div>
    </div>

    <footer>
        <p>Designed by: Sheik udhuman(25015367)</p>
    </footer>

</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #4CAF50;
            color: #ffffff;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            height: 80px;
        }

        header nav a {
            padding: 10px 15px;
            text-decoration: none;
            color: #ffffff;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease, background 0.3s ease;
            border-radius: 5px;
        }

        header nav a:hover {
            background: #ff5722;
            color: #ffffff;
        }

        .menu-container {
            padding: 20px;
            background: #f9f9f9;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 2.5rem;
            color: #333;
            margin-bottom: 20px;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .menu-item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .menu-item:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
        }

        .menu-details {
            padding: 15px;
        }

        .menu-details h3 {
            font-size: 1.5rem;
            color: #000000;
            margin-bottom: 8px;
        }

        .menu-details p {
            font-size: 1rem;
            color: #555;
            margin-bottom: 10px;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px 0;
            margin-top: 20px;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>AKS FOODIE HUB</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="owners.html" class="active">Owner</a>
        </nav>
    </header>

    <div class="menu-container">
        <h1>Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="biryani.png" alt="Biryani">
                <div class="menu-details">
                    <h3>Biryani</h3>
                    <p>Delicious spiced rice with meat.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="noodles.png" alt="Noodles">
                <div class="menu-details">
                    <h3>Noodles</h3>
                    <p>Stir-fried noodles with vegetables.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="chapathi.png" alt="Chapathi">
                <div class="menu-details">
                    <h3>Chapathi</h3>
                    <p>Soft Indian flatbread.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="momo.png" alt="Momo">
                <div class ="menu-details">
                    <h3>Momo</h3>
                    <p>Steamed dumplings filled with meat or vegetables.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="pasta.png" alt="Pasta">
                <div class="menu-details">
                    <h3>Pasta</h3>
                    <p>Italian pasta with a choice of sauces.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="burger.png" alt="Burger">
                <div class="menu-details">
                    <h3>Burger</h3>
                    <p>Juicy beef burger with fresh toppings.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="pizza.png" alt="Pizza">
                <div class="menu-details">
                    <h3>Pizza</h3>
                    <p>Classic pizza with cheese and toppings.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="wrap.png" alt="Wrap">
                <div class="menu-details">
                    <h3>Wrap</h3>
                    <p>Fresh vegetables and meat wrapped in a tortilla.</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="jamun.png" alt="Gulab Jamun">
                <div class="menu-details">
                    <h3>Gulab Jamun</h3>
                    <p>Sweet syrup-soaked dumplings.</p>
                </div>
            </div>
        
            <div class="menu-item">
                <img src="icecream.png" alt="Ice Cream">
                <div class="menu-details">
                    <h3>Ice Cream</h3>
                    <p>Delicious ice cream in various flavors.</p>
                </div>
            </div>
        </div>
    </div>
    
    <footer>
        <p>Designed by: Sheik udhuman(25015367)</p>
    </footer>
    
</body>
</html>

owners.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AKS Foods | Owner Akshuu Uzii</title>
  <style>
    /* === Global Reset === */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-color: #fffaf3;
      color: #3a2a20;
      line-height: 1.6;
    }

    /* === Header === */
    header {
      background-color: #6b1d1d;
      color: #f7e7ce;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      border-bottom: 4px solid #e37b40;
    }

    header h1 {
      font-family: 'Georgia', serif;
      font-size: 2rem;
      letter-spacing: 1px;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    header h1::before {
      content: "🔥";
      font-size: 1.8rem;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 1.5rem;
    }

    nav a {
      color: #f7e7ce;
      text-decoration: none;
      font-weight: 500;
      transition: 0.3s;
    }

    nav a:hover,
    nav a.active {
      border-bottom: 2px solid #f7e7ce;
    }

    /* === Owner Section === */
    .owner-section {
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 4rem 2rem;
    }

    .owner-card {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      max-width: 600px;
      background: #fff;
      border-radius: 20px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.15);
      overflow: hidden;
      border: 3px solid #e37b40;
      padding: 2rem;
    }

    /* === Small Owner Photo === */
    .owner-photo {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #e37b40;
      margin-bottom: 1rem;
    }

    .owner-info h2 {
      color: #6b1d1d;
      font-family: 'Georgia', serif;
      font-size: 1.8rem;
      margin-bottom: 0.5rem;
    }

    .owner-info h3 {
      font-size: 1.2rem;
      font-weight: 500;
      color: #e37b40;
      margin-bottom: 1rem;
    }

    .owner-info p {
      margin-bottom: 1rem;
      font-size: 1rem;
    }

    /* === Social Links === */
    .social-links {
      display: flex;
      justify-content: center;
      gap: 1rem;
      margin-top: 1rem;
    }

    .social-links img {
      width: 32px;
      height: 32px;
      transition: 0.3s;
      filter: sepia(40%) hue-rotate(-10deg);
    }

    .social-links img:hover {
      transform: scale(1.1);
      filter: none;
    }

    /* === Footer === */
    footer {
      background-color: #6b1d1d;
      color: #f7e7ce;
      text-align: center;
      padding: 1rem;
      font-size: 0.9rem;
      border-top: 4px solid #e37b40;
    }

    /* === Responsive === */
    @media (max-width: 768px) {
      .owner-card {
        width: 90%;
      }
    }
  </style>
</head>
<body>
  <!-- Header -->
  <header>
    <h1>AKS Foods</h1>
    <nav>
      <ul>
        <li><a href="home.html">Home</a></li>
        <li><a href="menu.html">Menu</a></li>
        <li><a href="contact.html">Contact</a></li>
        <li><a href="owners.html" class="active">Owner</a></li>
      </ul>
    </nav>
  </header>

  <!-- Owner Section -->
  <section class="owner-section">
    <div class="owner-card">
      <img src="akshuu.jpg" alt="Owner Akshuu Uzii" class="owner-photo">

      <div class="owner-info">
        <h2>Meet the Owner</h2>
        <h3>Akshuu Uzii</h3>
        <p>
          Welcome to <strong>AKS Foods</strong> — where passion meets flavor and every dish tells a story. 
          I’m <b>Akshuu Uzii</b>, the proud founder and heart behind our kitchen.
        </p>
        <p>
          Inspired by vintage tastes and fiery creativity, our restaurant combines classic comfort with bold, modern touches.
          Each flame in our kitchen represents our commitment to quality, warmth, and unforgettable taste.
        </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 AKS Foods | All Rights Reserved</p>
  </footer>
</body>
</html>
~~~

## OUTPUT:
![alt text](<Screenshot 2025-10-06 220144.png>)
![alt text](<Screenshot 2025-10-06 220327.png>)
![alt text](<Screenshot 2025-10-06 220427.png>)
![alt text](<Screenshot 2025-10-06 220442.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
