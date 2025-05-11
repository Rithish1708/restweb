# Ex.07 Restaurant Website
## Date:11/05/2025

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
res.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Roast & Toast</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background-image: url("bg2.jpg");
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            background-repeat: no-repeat;
        }

        header.banner {
            background-color: #222;
            color: white;
            padding: 20px 10px;
            text-align: center;
        }

        header.banner h1 {
            margin: 0;
            font-size: 2.5em;
            letter-spacing: 2px;
        }

        header.banner nav ul {
            list-style: none;
            padding: 0;
            margin: 10px 0 0;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        header.banner nav ul li {
            display: inline;
        }

        header.banner nav ul li a {
            text-decoration: none;
            color: white;
            font-size: 1.2em;
            transition: color 0.3s;
        }

        header.banner nav ul li a:hover {
            color: #ff6347;
        }

        section.intro {
            padding: 40px 20px;
            text-align: center;

            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin: 20px;
            border-radius: 10px;
        }

        section.intro h2 {
            font-size: 2em;
            color: #222;
            margin-bottom: 10px;
        }

        section.intro p {
            font-size: 1.1em;
            color: #100f0f;
            margin: 0;
        }

        footer {
            text-align: center;
            padding: 10px 0;
            background-color: #222;
            color: white;
            position: bottom;
            bottom: 0;
            width: 100%;
        }

        footer p {
            margin: 0;
            font-size: 0.9em;
        }

        @media (max-width: 768px) {
            header.banner nav ul {
                flex-direction: column;
                gap: 10px;
            }

            section.intro {
                margin: 10px;
            }
        }
    </style>
</head>

<body>
    <header class="banner">
        <h1>Welcome to Roast & Toast </h1>
        <nav>
            <ul>
                <li><a href="res.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="intro">
        <h2>Where every flavor tells a story.</h2>
        <h1>Hundreds of flavors under one roof.</h1>
    </section>
    <br><br><br><br><br><br><br><br><br><br><br><br><br><br>
    <footer>

        <p>© Rithish</p>
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
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            color: #333;
        }

        header.banner {
            background-color: #222;
            color: white;
            padding: 20px;
            text-align: center;
        }

        header.banner h1 {
            margin: 0;
        }

        header.banner nav ul {
            list-style: none;
            padding: 0;
            margin: 10px 0 0;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        header.banner nav ul li {
            display: inline;
        }

        header.banner nav ul li a {
            text-decoration: none;
            color: white;
            font-size: 1.2em;
            transition: color 0.3s;
        }

        header.banner nav ul li a:hover {
            color: #ff6347;
        }

        .menu {
            padding:5px;
            text-align: center;
        }

        .menu h2 {
            font-size: 2em;
            color: #222;
            margin-bottom: 1px;
        }

        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 10px;
            padding: 0;
        }

        .item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
            padding: 15px;
        }

        .item img {
            max-width: 100%;
            height: 50%;
            border-bottom: 1px solid #f4f4f4;
        }

        .item h3 {
            font-size: 1.5em;
            margin: 5px 0;
        }

        .item p {
            font-size: 1.2em;
            color: #555;
        }

        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 5px 0;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        footer p {
            margin: 0;
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <header class="banner">
        <h1>Menu</h1>
        <nav>
            <ul>
                <li><a href="res.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="menu">
        <h2>Our Delicious Menu</h2>
        <div class="menu-items">
            
            <div class="item">
                <img src="dal rice.jpg" alt="dhall rice">
                <h3>dhall rice</h3>
                <p>Rs.250</p>
            </div>
            <div class="item">
                <img src="macaroni.jpg" alt="macroni">
                <h3>macroni</h3>
                <p>Rs. 350</p>
            </div>
            <div class="item">
                <img src="fish.webp" alt="fish">
                <h3>fish</h3>
                <p>Rs. 500</p>
            </div>

            <div class="item">
                <img src="biriyani.webp" alt="briyani">
                <h3>briyani </h3>
                <p>Rs. 400</p>
            </div>

            <div class="item">
                <img src="keema roll.jpg" alt="keema roll">
                <h3>keema roll</h3>
                <p>Rs. 300</p>
            </div>

            <div class="item">
                <img src="samosa.webp" alt="samosa">
                <h3>samosa</h3>
                <p>Rs. 25</p>
            </div>

            <div class="item">
                <img src="fries.jpg" alt="fries">
                <h3>fries</h3>
                <p>Rs. 250</p>
            </div>

            <div class="item">
                <img src="noodles.webp" alt="noodles">
                <h3>noodles</h3>
                <p>Rs. 200</p>
            </div>

            <div class="item">
                <img src="dosa.webp" alt="dosa">
                <h3>dosa</h3>
                <p>Rs. 120</p>
            </div>
            <div class="item">
                <img src="pori.jpg" alt="poori">
                <h3>poori</h3>
                <p>Rs. 130</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Rithish</p>
    </footer>
</body>
</html>

administration.html

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
            background-color: #f4f4f4;
            color: #333;
        }

        .banner {
            background-color: #131413;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        .banner h1 {
            margin: 0;
            font-size: 2.5em;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            background-color: #333;
        }

        nav ul li {
            margin: 0;
        }

        nav ul li a {
            display: block;
            padding: 10px 20px;
            text-decoration: none;
            color: white;
        }

        nav ul li a:hover {
            color: red;
        }

        .team {
            padding: 40px 20px;
            text-align: center;
        }

        .team h2 {
            margin-bottom: 20px;
            font-size: 2em;
            color: #4CAF50;
        }

        .team-members {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .member {
            background: white;
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            width: 200px;
            padding: 20px;
            text-align: center;
        }

        .member img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 15px;
        }

        .member h3, .member h4, .member h5, .member h6 {
            margin: 10px 0 5px;
            font-size: 1.2em;
            color: #333;
        }

        .member p {
            margin: 0;
            font-size: 0.9em;
            color: #666;
        }

        footer {
            text-align: center;
            background-color: #333;
            color: white;
            padding: 10px 0;
            margin-top: 220px;
        }
    </style>
</head>
<body>
    <header class="banner"> 
        <h1>Our Team</h1>
        <nav>
            <ul>
                <li><a href="res.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="team">        <h2>Meet Our Team</h2>
        <div class="team-members">
            <div class="member">
                <img src="Damodharan k.jpg" alt="K. Damodharan">
                <h3>K. Damodharan</h3>
                <p>owner</p>
            </div>
            <div class="member">
                <img src="venk.jpg" alt="chef venkatesh bhat">
                <h3>chef venkatesh bhat</h3>
                <p>Chef</p>
            </div>
            <div class="member">
                <img src="pugazhal.jpg" alt="Madhampatty Rangaraj">
                <h3>pugzhal</h3>
                <p>manager</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Rithish</p>
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
            background-color: #f4f4f4;
            color: #333;
        }

        .banner {
            background-color: #0f100f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        .banner h1 {
            margin: 0;
            font-size: 2.5em;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            background-color: #333;
        }

        nav ul li {
            margin: 0;
        }

        nav ul li a {
            display: block;
            padding: 10px 20px;
            text-decoration: none;
            color: white;
        }

        nav ul li a:hover {
            color: red;
        }

        .contact {
            padding: 40px 20px;
            text-align: center;
        }

        .contact h2 {
            margin-bottom: 20px;
            font-size: 2em;
            color: #4CAF50;
        }

        .contact p {
            font-size: 1.2em;
            margin: 10px 0;
            color: #555;
        }

        footer {
            text-align: center;
            background-color: #333;
            color: white;
            padding: 10px 0;
            margin-top: 24%;
        }
    </style>
</head>
<body>
    <header class="banner">
        <h1>Contact Us</h1>
        <nav>
            <ul>
                <li><a href="res.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="contact">
        <h2>Get in Touch</h2>
        <p><strong>Address:</strong>No.86, Block No.5, Manickam Lane, Anna Salai, Guindy, Chennai, Tamil Nadu 600032</p>
        <p><strong>Phone:</strong>8756784742</p>
        <p><strong>Email:</strong> rithishrestaurant@gmail.com</p>
    </section>

    <footer>
        <p>&copy; 2025 Rithish</p>
    </footer>
</body>
</html>

style.css

body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
    background-image: url("C:\Users\admin\Pictures\bg.jpg"); /* Replace with your image file path */
    background-size: cover; 
    background-position: center; 
    background-attachment: fixed; 
    background-repeat: no-repeat; 
}

header.banner {
    background-color: #222;
    color: white;
    padding: 20px 10px;
    text-align: center;
}

header.banner h1 {
    margin: 0;
    font-size: 2.5em;
    letter-spacing: 2px;
}

header.banner nav ul {
    list-style: none;
    padding: 0;
    margin: 10px 0 0;
    display: flex;
    justify-content: center;
    gap: 20px;
}

header.banner nav ul li {
    display: inline;
}

header.banner nav ul li a {
    text-decoration: none;
    color: white;
    font-size: 1.2em;
    transition: color 0.3s;
}

header.banner nav ul li a:hover {
    color: #ff6347;
}

section.intro {
    padding: 40px 20px;
    text-align: center;
   
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    margin: 20px;
    border-radius: 10px;
}

section.intro h2 {
    font-size: 2em;
    color: #222;
    margin-bottom: 10px;
}

section.intro p {
    font-size: 1.1em;
    color: #100f0f;
    margin: 0;
}

footer {
    text-align: center;
    padding: 10px 0;
    background-color: #222;
    color: white;
    position: bottom;
    bottom: 0;
    width: 100%;
}

footer p {
    margin: 0;
    font-size: 0.9em;
}

@media (max-width: 768px) {
    header.banner nav ul {
        flex-direction: column;
        gap: 10px;
    }

    section.intro {
        margin: 10px;
    }
}

```

## OUTPUT:
![alt text](<Screenshot (34).png>)
![alt text](<Screenshot (35).png>)
![alt text](<Screenshot (36).png>)
![alt text](<Screenshot (37).png>)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
