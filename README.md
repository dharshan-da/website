# Ex.07 Restaurant Website
# Date:12-11-2014
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
project.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Chocolate | shop </title>
    <style>
        *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;

}

.container{
  height: 100vh;
  width:100% ;
    background: linear-gradient(rgba(48, 32, 32, 0.605),rgba(179, 178, 172, 0.7)),url(tablefood.avif);
    background-size: cover  ;
    background-position: center;
    font-family: "Apple" "Chancery", "cursive";
}
.nav-bar{
    display: flex;
    align-items: center;
    justify-content: space-between ;
    padding: 30px 80px;  
}
.nav-bar  .title{
    color: lemonchiffon;
    font size: 67px;
    font-weight:700;
    cursor: pointer;
}       
 
span{
    color: rgb(223, 232, 124);
}
.menu li{
    list-style: none;
    display: inline-block;
}
.menu li a{
    text-decoration: none;
    color: white;
    font-size: 27px;
    margin-left: 25px;
    font-weight: 600;
    transition: .4s  ease;
}
    
.menu li a:hover{
    color:lemonchiffon;
    padding: 5px 10px;
    border: 2px solid white;
}
.home{
    height: 400px;
    padding: 70px;
}
.title-1{
    font-size: 56px;
    color: lemonchiffon;
    font-weight: 600;
}

.home p{
    color: lemonchiffon;
    font-size: 20px;
    padding-top: 10px;
}
.home button{
    height: 40px;
    color: white;
    background: crimson;
    padding: 5px 30px;
    margin-top: 20px;
    border: none;
    border-radius: 5px;
    font-size: 22px;
    transition: .4s ease;
    cursor: pointer;
}
.home button:hover{
    background: none;
    border: 2px solid crimson;
}
    </style>
</head>
<body>
     <div class="container">
        <div class="nav-bar">
            <h1 class="title">spicy<span>Food</span></h1>
            <ul class="menu">
                <li><a href="ocean_food.html">FOOD MENU</a></li>
                <li><a href="contact.html">CONTACT</a></li>
                <li><a href="order.html">ORDER</a></li>
                <li><a href="adminstration.html">ADMINISTARTION</a></li>
            </ul>
        </div>

        <div class="home">
            <h1 class="title-1">Good <span>Food</span> will always <br> Find the audience</h1>
            <p>We provide a variety of uniques and best Food</p>
            
        </div>



     </div>
</body>
</html>

administration.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Hotel Administration - Chefs</title>
</head>
<style>
    /* General Styles */
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  margin: 0;
  display: flex;
  flex-direction: column;
  height: 100vh;
}

header {
  background-color: #007bff;
  color: #fff;
  padding: 10px 0;
}

.container {
  width: 90%;
  margin: 0 auto;
  flex: 1;
}

header h1 {
  text-align: center;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  padding: 0;
}

nav ul li {
  margin: 0 15px;
}

nav ul li a {
  text-decoration: none;
  color: #fff;
  font-weight: bold;
}

nav ul li a:hover {
  color: #e0e0e0;
}

/* Main Content */
main {
  padding: 20px;
}

h2 {
  text-align: center;
  margin-bottom: 20px;
}

.chef-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

.chef-card {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  text-align: center;
  padding: 15px;
}

.chef-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 8px;
}

.chef-card h3 {
  margin: 10px 0;
  color: #333;
}

.chef-card p {
  color: #777;
}

/* Footer */
footer {
  background-color: #007bff;
  color: #fff;
  text-align: center;
  padding: 10px 0;
}

</style>
<body>
  <header>
    <div class="container">
      <h1>Hotel Administration</h1>
      <nav>
        <ul>
          <li><a href="#">Dashboard</a></li>
          <li><a href="#">Bookings</a></li>
          <li><a href="#">Chefs</a></li>
          <li><a href="#">Rooms</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <div class="container">
    <main>
      <h2>Chefs Overview</h2>
      <section class="chef-grid">
        <!-- Chef 1 -->
        <div class="chef-card">
          <img src="chef1.png" alt="Chef 1" />
          <h3>Chef 1</h3>
          <p>Specialty: Italian Cuisine</p>
        </div>
        <!-- Chef 2 -->
        <div class="chef-card">
          <img src="chef2.jpg" alt="Chef 2" />
          <h3>Chef 2</h3>
          <p>Specialty: French Pastry</p>
        </div>
        <!-- Chef 3 -->
        <div class="chef-card">
          <img src="chef3.jpg" alt="Chef 3" />
          <h3>Chef 3</h3>
          <p>Specialty: Asian Fusion</p>
        </div>
        <!-- Chef 4 -->
        <div class="chef-card">
          <img src="chef4.jpg" alt="Chef 4" />
          <h3>Chef 4</h3>
          <p>Specialty: Vegan Dishes</p>
        </div>
        <!-- Chef 5 -->
        <div class="chef-card">
          <img src="chef5.jpeg" alt="Chef 5" />
          <h3>Chef 5</h3>
          <p>Specialty: Seafood</p>
        </div>
        <!-- Chef 6 -->
        <div class="chef-card">
          <img src="chef6.webp" alt="Chef 6" />
          <h3>Chef 6</h3>
          <p>Specialty: Barbecue</p>
        </div>
       
      </section>
    </main>
  </div>

  <footer>
    <div class="container">
      <p>&copy; 2024 Hotel Administration. All rights reserved.</p>
    </div>
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
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
        }

        .container {
            max-width: 800px;
            margin: 50px auto;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 20px;
        }

        h1 {
            text-align: center;
            color: #333;
        }

        form {
            display: flex;
            flex-direction: column;
        }

        label {
            margin: 10px 0 5px;
            font-weight: bold;
            color: #555;
        }

        input, textarea {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
            width: 100%;
        }

        textarea {
            resize: vertical;
            min-height: 100px;
        }

        button {
            margin-top: 20px;
            padding: 10px 15px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }

        .contact-info {
            margin-top: 30px;
            text-align: center;
        }

        .contact-info p {
            margin: 5px 0;
            color: #666;
        }

        .contact-info a {
            color: #007BFF;
            text-decoration: none;
        }

        .contact-info a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Contact Us</h1>
        <form action="/submit" method="POST">
            <label for="name">Name</label>
            <input type="text" id="name" name="name" placeholder="Your Name" required>

            <label for="email">Email</label>
            <input type="email" id="email" name="email" placeholder="Your Email" required>

            <label for="message">Message</label>
            <textarea id="message" name="message" placeholder="Your Message" required></textarea>

            <button type="submit">Send Message</button>
        </form>

        <div class="contact-info">
            <p>Phone: <a href="tel:+1234567890">+91 7305156131</a></p>
            <p>Email: <a href="mailto:info@example.com">rajashri56131@gmail.com</a></p>
            <p>Address: saveetha engineering college </p>
        </div>
    </div>
</body>
</html>


ocean-food.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fdfaf6;
        }

        .container {
            max-width: 900px;
            margin: 50px auto;
            padding: 20px;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        h1 {
            text-align: center;
            color: #333;
            margin-bottom: 20px;
        }

        .menu {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .menu-item {
            background-color: #fffaf0;
            border: 1px solid #f0e5d8;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            transition: transform 0.2s;
        }

        .menu-item:hover {
            transform: scale(1.05);
        }

        .menu-item img {
            width: 100%;
            height: 150px;
            object-fit: cover;
        }

        .menu-item-content {
            padding: 15px;
            text-align: center;
        }

        .menu-item h2 {
            font-size: 18px;
            margin: 10px 0;
            color: #444;
        }

        .menu-item p {
            font-size: 14px;
            color: #666;
            margin: 10px 0;
        }

        .menu-item span {
            display: block;
            margin-top: 10px;
            font-size: 16px;
            font-weight: bold;
            color: #e67e22;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Our Menu</h1>
        <div class="menu">
            <div class="menu-item">
                <img src="grill.jpeg" alt="Dish 1">
                <div class="menu-item-content">
                    <h2>Grilled Chicken</h2>
                    <p>Juicy grilled chicken served with fresh vegetables.</p>
                    <span>$12.99</span>
                </div>
            </div>

            <div class="menu-item">
                <img src="vegan salad.jpg" alt="Dish 2">
                <div class="menu-item-content">
                    <h2>Vegan Salad</h2>
                    <p>A healthy mix of greens, fruits, and nuts.</p>
                    <span>$9.99</span>
                </div>
            </div>

            <div class="menu-item">
                <img src="spaghetti.jpg" alt="Dish 3">
                <div class="menu-item-content">
                    <h2>Spaghetti Bolognese</h2>
                    <p>Classic Italian pasta with a rich meat sauce.</p>
                    <span>$11.99</span>
                </div>
            </div>

            <div class="menu-item">
                <img src="burger.jpg" alt="Dish 4">
                <div class="menu-item-content">
                    <h2>Cheeseburger</h2>
                    <p>A hearty burger with cheese, lettuce, and tomato.</p>
                    <span>$10.49</span>
                </div>
            </div>

            <div class="menu-item">
                <img src="pizza.jpg" alt="Dish 5">
                <div class="menu-item-content">
                    <h2>Margherita Pizza</h2>
                    <p>Classic pizza topped with tomato, mozzarella, and basil.</p>
                    <span>$13.49</span>
                </div>
            </div>

            <div class="menu-item">
                <img src="sushi.jpg" alt="Dish 6">
                <div class="menu-item-content">
                    <h2>Sushi Platter</h2>
                    <p>Assorted fresh sushi rolls with wasabi and soy sauce.</p>
                    <span>$18.99</span>
                </div>
            </div>

            <div class="menu-item">
                <img src="choco cake.jpg" alt="Dish 7">
                <div class="menu-item-content">
                    <h2>Chocolate Cake</h2>
                    <p>Rich and moist chocolate cake with a creamy frosting.</p>
                    <span>$6.99</span>
                </div>
            </div>

            <div class="menu-item">
                <img src="smoothie.jpg" alt="Dish 8">
                <div class="menu-item-content">
                    <h2>Fruit Smoothie</h2>
                    <p>Refreshing blend of seasonal fruits and yogurt.</p>
                    <span>$5.49</span>
                </div>
            </div>
        </div>
    </div>
</body>
</html>


order.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Order Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
        }

        .container {
            max-width: 800px;
            margin: 50px auto;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 20px;
        }

        h1 {
            text-align: center;
            color: #333;
        }

        form {
            display: flex;
            flex-direction: column;
        }

        label {
            margin: 10px 0 5px;
            font-weight: bold;
            color: #555;
        }

        input, select {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
            width: 100%;
        }

        button {
            margin-top: 20px;
            padding: 10px 15px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
        }

        button:hover {
            background-color: #218838;
        }

        .summary {
            margin-top: 30px;
            padding: 15px;
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 4px;
        }

        .summary p {
            margin: 5px 0;
            font-size: 16px;
            color: #555;
        }

        .summary span {
            font-weight: bold;
            color: #000;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Place Your Order</h1>
        <form action="/submit-order" method="POST">
            <label for="name">Name</label>
            <input type="text" id="name" name="name" placeholder="Your Name" required>

            <label for="email">Email</label>
            <input type="email" id="email" name="email" placeholder="Your Email" required>

            <label for="phone">Phone</label>
            <input type="tel" id="phone" name="phone" placeholder="Your Phone Number" required>

            <label for="address">Address</label>
            <input type="text" id="address" name="address" placeholder="Your Address" required>

            <label for="item">Select Item</label>
            <select id="item" name="item" required>
                <option value="">-- Select a Food Item --</option>
                <option value="grilled-chicken">Grilled Chicken - $12.99</option>
                <option value="vegan-salad">Vegan Salad - $9.99</option>
                <option value="spaghetti">Spaghetti Bolognese - $11.99</option>
                <option value="cheeseburger">Cheeseburger - $10.49</option>
                <option value="pizza">Margherita Pizza - $13.49</option>
                <option value="sushi">Sushi Platter - $18.99</option>
                <option value="chocolate-cake">Chocolate Cake - $6.99</option>
                <option value="smoothie">Fruit Smoothie - $5.49</option>
            </select>

            <label for="quantity">Quantity</label>
            <input type="number" id="quantity" name="quantity" min="1" placeholder="Enter Quantity" required>

            <button type="submit">Submit Order</button>
        </form>

        <div class="summary">
            <p><span>Note:</span> Please ensure all details are correct before submitting your order.</p>
            <p><span>Delivery:</span> Orders are typically delivered within 30-45 minutes.</p>
        </div>
    </div>
</body>
</html>



```

# OUTPUT:

![res pic](https://github.com/user-attachments/assets/5af8a01f-0f10-497e-9285-549367155ede)

![res menu](https://github.com/user-attachments/assets/551b161e-d78b-46cf-a08e-14764e8ce69b)

![res cc contact](https://github.com/user-attachments/assets/6d215656-65e6-4bc0-9061-80b85afe09f1)

![res contact us](https://github.com/user-attachments/assets/778f9a62-c155-4c93-9886-dab92a851ab4)

![res order cc](https://github.com/user-attachments/assets/a1794a76-0ccd-40a8-91ff-d3aa1fd13ec6)

![res order](https://github.com/user-attachments/assets/795b04ee-7dfb-4493-98c1-b796ba386fd8)

![res admin cc](https://github.com/user-attachments/assets/0f2cdb71-1384-44e5-bbca-e407e355b849)

![res administration](https://github.com/user-attachments/assets/4c703368-a827-4425-9401-ce29c72cbdf0)



# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
