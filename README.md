# Project Responsive Web Design using Bootstrap
## Date:19.12.2024

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Design Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="top-bar">
        <input type="text" class="search-bar" placeholder="Search...">
        <a href="#" class="nav-item">Explore</a>
        <a href="#" class="nav-item">Hire a Designer</a>
        <a href="#" class="nav-item">Find Jobs</a>
        <a href="#" class="nav-item">Blog</a>
        <a href="#" class="nav-item blue-text">Sign up</a>
        <a href="#" class="nav-item blue-text">Log in</a>
    </div>

    <header>
        <div class="header-content">
            <h1>Discover the world’s top designers</h1>
            <p>Explore work from the most talented and accomplished designers ready to take on your next project</p>
            <input type="text" class="search-input" placeholder="What are you looking for?">
        </div>
    </header>

    <section class="trending">
        <h2>Trending Searches</h2>
        <div class="trending-tags">
            <span>landing page</span>
            <span>e-commerce</span>
            <span>mobile app</span>
            <span>logo design</span>
            <span>dashboard</span>
            <span>icons</span>
        </div>
    </section>

    <section class="gallery">

        <div class="card">
            <img src="4.jpg" alt="Design Sample">
            <h3>Momos</h3>
            <p>HR Team | 9.2k Views</p>
        </div>

        <div class="card">
            <img src="3.jpg" alt="Design Sample">
            <h3>Fried Chicken</h3>
            <p>HR Team | 10.2k Views</p>
        </div>

        <div class="card">
            <img src="9.jpg" alt="Design Sample">
            <h3>Pizza</h3>
            <p>HR Team | 6.2k Views</p>
        </div>

        <div class="card">
            <img src="7.jpg" alt="Design Sample">
            <h3>Chocolate Shake</h3>
            <p>HR Team | 13.2k Views</p>
        </div>

        <div class="card">
            <img src="6.jpg" alt="Design Sample">
            <h3>Kuanfa</h3>
            <p>HR Team | 15.2k Views</p>
        </div>

        <div class="card">
            <img src="8.jpg" alt="Design Sample">
            <h3>Strawberry Cake</h3>
            <p>HR Team | 8.2k Views</p>
        </div>

        <div class="card">
            <img src="2.jpg" alt="Design Sample">
            <h3>Falooda</h3>
            <p>HR Team | 16.2k Views</p>
        </div>

        <div class="card">
            <img src="5.jpg" alt="Design Sample">
            <h3>Pista Shake</h3>
            <p>HR Team | 10.2k Views</p>
        </div>

        <div class="card">
            <img src="10.jpg" alt="Design Sample">
            <h3>Oreo Icecream</h3>
            <p>HR Team | 9.2k Views</p>
        </div>

        <div class="card">
            <img src="11.jpg" alt="Design Sample">
            <h3>Chocobar</h3>
            <p>HR Team | 14.4k Views</p>
        </div>

        <div class="card">
            <img src="12.jpg" alt="Design Sample">
            <h3>Paneer Noodles</h3>
            <p>HR Team | 13.2k Views</p>
        </div>

        <div class="card">
            <img src="1.jpg" alt="Design Sample">
            <h3>Sandwich And Fries</h3>
            <p>HR Team | 16.2k Views</p>
        </div>
        
    </section>

    
    <footer>
        <p>&copy; 2024 Design Portfolio!All rights reserved.</p>
        <p>Designed And Developed By:Hari Ram (24005836)</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

style.css

body, h1, h2, p, a, input, button {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f5f5f5;
    color: #333;
}

.top-bar {
    display: flex;
    align-items: center;
    background-color: #ffffff;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.search-bar {
    margin-right: 15px;
    padding: 8px;
    border: 1px solid #ddd;
    border-radius: 4px;
    outline: none;
}

.nav-item {
    margin: 0 10px;
    color: #333;
    text-decoration: none;
}

.blue-text {
    color: #007bff;
    font-weight: bold;
}

.blue-text:hover {
    text-decoration: underline;
}

header {
    background-image: url('bg1.jpg'); 
    background-size: cover;
    padding: 80px 20px;
    text-align: center;
    color: #fff;
}

.header-content h1 {
    font-size: 36px;
    margin-bottom: 10px;
}

.header-content p {
    font-size: 18px;
    margin-bottom: 20px;
}

.search-input {
    padding: 10px;
    width: 60%;
    max-width: 500px;
    border: none;
    border-radius: 4px;
    outline: none;
}

.trending {
    padding: 20px;
    text-align: center;
}

.trending h2 {
    font-size: 24px;
    margin-bottom: 10px;
}

.trending-tags {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.trending-tags span {
    background-color: #007bff;
    color: #fff;
    padding: 5px 10px;
    margin: 5px;
    border-radius: 4px;
    font-size: 14px;
}

.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
}

.card img {
    width: 100%;
    height: auto;
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
    position: relative;
}

.card img {
    width: 100%;
    height: auto;
    transition: transform 0.3s ease;
}

.card:hover img {
    transform: scale(1.2); 
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 20px;
    margin-top: 20px;
}

script.js

const searchBar = document.querySelector('.search-bar');

searchBar.addEventListener('keydown', function(event) {
    if (event.key === 'Enter') {
        event.preventDefault(); 
        alert(`Searching for: ${searchBar.value}`);
    }
});
```

## OUTPUT:
![alt text](<Screenshot 2024-12-19 194459-1.png>)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
