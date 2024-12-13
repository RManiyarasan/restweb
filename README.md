# Ex.07 Restaurant Website
## Date:13.12.24

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
```
rest.html 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome to Our Restaurant</title>
    <style>

        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background-color:rebeccapurple
        }

     
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #333;
            padding: 10px 20px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.1em;
        }

        nav a:hover {
            color: #f39c12;
        }

        .banner {
            height: 100vh;
            background: url('banner2.jpg') no-repeat center center/cover;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
        }

        .banner h1 {
            font-size: 4em;
            margin: 0;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }

        .banner p {
            font-size: 1.5em;
            margin: 20px 0;
            max-width: 600px;
            line-height: 1.5;
        }

        .banner a {
            padding: 15px 30px;
            background-color: #f39c12;
            color: white;
            font-size: 1.2em;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        .banner a:hover {
            background-color: #d35400;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 15px;
            font-size: 1em;
        }
    </style>
</head>
<body>

  
    <nav>
        <div>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="admin.html">Administration</a>
            <a href="contact.html">Contact Us</a>
        </div>
    </nav>

   
    <div class="banner">
        <h1>Shiva's Restaurant</h1>
        <p>
            Discover the finest dining experience with exquisite flavors, exceptional service, 
            and a warm atmosphere that will leave you wanting more.
        </p>
    </div>        

    <footer>
        <p>Designed by [Your Name] &copy; 2024</p>
    </footer>

</body>
</html>

home.html

 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Home</title>
    <style>
   
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fafafa;
        }

        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 40px;
        }

        header h1 {
            margin: 0;
            font-size: 2.5em;
        }

        header p {
            margin: 10px 0;
            font-size: 1.2em;
        }

        .intro {
            text-align: center;
            padding: 20px;
            background-color: #f4f4f4;
            color: #555;
        }

        .intro h2 {
            margin: 10px 0;
        }

        .intro p {
            margin: 0;
            font-size: 1.1em;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            padding: 20px;
        }

        .gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            transition: transform 0.3s ease;
        }

        .gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to Shiva's restaurant</h1>
        <p>Where Flavor Meets Elegance</p>
    </header>

    <div class="intro">
        <h2>Our Signature Dishes</h2>
        <p>Explore the best meals handpicked by our top chefs.</p>
    </div>

    <div class="gallery">
        
        <img src="Dosai.jpg" alt="">
        
        <img src="Idly.jpg" alt="">
        
        <img src="mutton.jpg" alt="">
        
        <img src="chicken.jpg"alt="">
       
    </div>

    <footer>
        <p>Designed by shiva &copy; 2024</p>
    </footer>

</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Menu</title>
    <style>
        /* General Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color:dimgray;
            color: white;
            text-align: center;
            padding: 40px;
        }

        header h1 {
            margin: 0;
            font-size: 2.5em;
        }

        header p {
            margin: 10px 0;
            font-size: 1.2em;
        }

        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .menu-item {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .menu-item:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .menu-item-content {
            padding: 15px;
            text-align: center;
        }

        .menu-item-content h3 {
            margin: 10px 0;
            font-size: 1.5em;
            color: #333;
        }

        .menu-item-content p {
            margin: 5px 0;
            font-size: 1em;
            color: #666;
        }

        .menu-item-content .price {
            font-size: 1.2em;
            color: #d35400;
            font-weight: bold;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Our Menu</h1>
        <p>Explore the flavors of our finest dishes</p>
    </header>

    <div class="container">
        <div class="menu-grid">
           
            <div class="menu-item">
                <img src="Dosai.jpg" alt="Dosai">
                <div class="menu-item-content">
                    <h3>Dosai</h3>
                    <p>Crispy Dosai</p>
                    <p class="price">Rs.30</p>
                </div>
            </div>


            <div class="menu-item">
                <img src="Idly.jpg" alt="Idly">
                <div class="menu-item-content">
                    <h3>Idly</h3>
                    <p>Special idly</p>
                    <p class="price">Rs.10</p>
                </div>
            </div>

            
            <div class="menu-item">
                <img src="chicken.jpg" alt="Chicken gravy">
                <div class="menu-item-content">
                    <h3>Chicken gravy</h3>
                    <p>Spicy chicken gravy.</p>
                    <p class="price">Rs.100</p>
                </div>
            </div>

            
            <div class="menu-item">
                <img src="mutton.jpg" alt="Mutton gravy">
                <div class="menu-item-content">
                    <h3>Mutton gravy</h3>
                    <p>Delicious mutton gravy</p>
                    <p class="price">Rs.199</p>
                </div>
            </div>

           
            
            </div>

            
            
            </div>
        </div>
    </div>

    <footer>
        <p>Designed by [Your Name] &copy; 2024</p>
    </footer>

</body>
</html>

admin.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration</title>
    <style>
       
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
            color: #333;
        }

        header {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 40px;
        }

        header h1 {
            margin: 0;
            font-size: 2.5em;
        }

        header p {
            margin: 10px 0;
            font-size: 1.2em;
        }

        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
        }

        .team-member {
            display: flex;
            align-items: center;
            background-color: white;
            margin: 15px 0;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .team-member img {
            width: 120px;
            height: 120px;
            object-fit: cover;
            border-radius: 8px;
            margin-right: 20px;
        }

        .team-details {
            flex: 1;
        }

        .team-details h3 {
            margin: 0 0 10px;
            color: #2c3e50;
        }

        .team-details p {
            margin: 2px 0;
            font-size: 1.1em;
            color: #555;
        }

        .team-divider {
            height: 2px;
            background-color: #2c3e50;
            margin: 2px 0;
        }

        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Our Administration Team</h1>
        <p>Passionate individuals who run our restaurant</p>
    </header>

    <div class="container">

        
        <div class="team-member">
            <img src="ak.jpg" alt="Admin 1">
            <div class="team-details">
                <h3>Akash</h3>
                <p>Restaurant Manager</p>
                <p>With 10+ years of experience in hospitality, Akash ensures smooth operations and excellent customer experiences.</p>
            </div>
        </div>
        <div class="team-divider"></div>

        <div class="team-member">
            <img src="maniii.jpg" alt="Admin 2">
            <div class="team-details">
                <h3>Maniyarsan</h3>
                <p>Head Chef</p>
                <p>An expert in creating mouth-watering dishes, Maniyarsan leads the culinary team with creativity and precision.</p>
            </div>
        </div>
        <div class="team-divider"></div>

        <div class="team-member">
            <img src="sachu.jpg" alt="Admin 3">
            <div class="team-details">
                <h3>Saravedi Sachin</h3>
                <p>Operations Manager</p>
                <p>Sachin oversees daily operations to maintain quality and efficiency in all aspects of the restaurant.</p>
            </div>
        </div>
        <div class="team-divider"></div>

        

       

    </div>

    <footer>
        <p>Designed by [Your Name] &copy; 2024</p>
    </footer>

</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        /* General Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f9fa;
        }

        header {
            background-color:black;
            color: white;
            text-align: center;
            padding: 30px;
        }

        header h1 {
            margin: 0;
            font-size: 2.5em;
        }

        header p {
            margin: 10px 0;
            font-size: 1.2em;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .contact-info, .contact-form {
            background-color: white;
            padding: 20px;
            margin: 20px 0;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .contact-info {
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .contact-info div {
            flex: 1;
        }

        .contact-info h3 {
            margin: 0;
            color:black;
        }

        .contact-info p {
            margin: 5px 0;
            font-size: 1.1em;
        }

        .contact-info img {
            width: 80px;
            height: 80px;
        }

        .contact-form h3 {
            margin-bottom: 20px;
            color: #333;
        }

        .contact-form form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .contact-form input, .contact-form textarea {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1em;
            width: 100%;
        }

        .contact-form button {
            padding: 10px;
            background-color:black;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1em;
            cursor: pointer;
        }

        .contact-form button:hover {
            background-color:black;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Contact Us</h1>
        <p>We'd love to hear from you!</p>
    </header>

    <div class="container">

        <!-- Contact Information -->
        <div class="contact-info">
            <div>
                <h3>Visit Us</h3>
                <p>32/4 opposite to saveetha medical college,chennai.</p>
            </div>
            <div>
                <h3>Call Us</h3>
                <p>8765432109,9087654321</p>
            </div>
            <div>
                <h3>Email Us</h3>
                <p>shivarestaurant@gmail.com</p>
            </div>
        </div>

        <!-- Contact Form -->
        <div class="contact-form">
            <h3>Send Us a Message</h3>
            <form action="#">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
                <button type="submit">Submit</button>
            </form>
        </div>

    </div>

    <footer>
        <p>Designed by shiva &copy; 2024</p>
    </footer>

</body>
</html>

```


## OUTPUT:

![alt text](shiva/restapp/static/1.1.png)
![alt text](shiva/restapp/static/1.2.png)
![alt text](shiva/restapp/static/1.3.png)
![alt text](shiva/restapp/static/1.4.png)
![alt text](shiva/restapp/static/1.5.png)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
