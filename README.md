# MDAP-EX_01-Portfolio
## Date:11/08/2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
#### index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <nav>
            <div class="logo">Portfolio</span></div>
            <ul class="nav-links">
                <li><a href="#intro">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

   
    <section id="intro" class="hero">
        <h1>Hi, I'm <span>Rahul</span></h1>
        <p>I am a passionate Web Developer eager to create impactful and beautiful designs.</p>
        <a href="#projects" class="btn">View Projects</a>
    </section>

    <section id="about" class="about">
        <h2>About Me</h2>
        <p>
            Hi! I'm a web developer with skills in <span>HTML</span>, <span>CSS</span>, and <span>JavaScript</span>. 
            I love creating interactive and user-friendly websites.Making code that’s easy to use and nice to see.


        </p>
    </section>

    <section id="projects" class="projects">
        <h2>Projects</h2>
        <div class="project-container">
            <div class="project-box">
                <h3>Movie app</h3>
                <p>A website about movie updates implemented using html and css.</p>
                <a href="#" class="btn">View Project</a>
            </div>
            <div class="project-box">
                
                <h3>Grocery app</h3>
                <p>A website for a simple grocery shop to calculate price</p>
                <a href="#" class="btn">View Project</a>
            </div>
            
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <p><i class="fas fa-envelope"></i> Email: rahul@example.com</p>
        <p><i class="fas fa-phone-alt"></i> Phone: +123 456 789</p>
        <p><i class="fab fa-linkedin"></i> <a href="#">LinkedIn</a></p>
        <p><i class="fab fa-github"></i> <a href="#">GitHub</a></p>
    </section>

</body>
</html>
```
#### style.css
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: linear-gradient(to right, #1e1e2f, #282846);
    color: #f4f4f4;
    line-height: 1.6;
}

a {
    color: inherit;
    text-decoration: none;
}

header {
    background: rgba(0, 0, 0, 0.85);
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 3px 12px rgba(0,0,0,0.4);
}

nav {
    width: 90%;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.8rem;
    font-weight: bold;
    color: #00e6ff;
}

.logo span {
    color: #ff4ecd;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin-left: 25px;
}

.nav-links a {
    font-weight: bold;
    transition: color 0.3s ease, border-bottom 0.3s ease;
    border-bottom: 2px solid transparent;
}

.nav-links a:hover {
    color: #00e6ff;
    border-bottom: 2px solid #00e6ff;
}

.btn {
    display: inline-block;
    padding: 0.6rem 1.2rem;
    background: linear-gradient(135deg, #032f34, #0077ff);
    color: #fff;
    font-weight: bold;
    border-radius: 8px;
    transition: all 0.3s ease;
}

.btn:hover {
    background: linear-gradient(135deg, #ff4ecd, #b300ff);
    transform: translateY(-3px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
}

.hero {
    text-align: center;
    padding: 4rem 10%;
    background: linear-gradient(135deg, #23575d, #0077ff);
    border-radius: 0;
    color: #fff;
}

.hero h1 {
    font-size: 2.8rem;
    margin-bottom: 1rem;
}

.hero h1 span {
    color: lightblue;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.about {
    background: rgba(255, 255, 255, 0.05);
    padding: 3rem 10%;
    border-radius: 12px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.3);
}

.about span {
    color: #00e6ff;
}

.projects {
    text-align: center;
}

.project-container {
    display: flex;
    gap: 25px;
    flex-wrap: wrap;
    justify-content: center;
    margin-top: 2rem;
}

.project-box {
    background: #1b1b2f;
    border-radius: 12px;
    overflow: hidden;
    width: 300px;
    text-align: center;
    box-shadow: 0 4px 15px rgba(0,0,0,0.4);
    transform: translateY(0);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-box img {
    width: 100%;
    display: block;
}

.project-box h3 {
    margin: 0.8rem 0;
    color: #00e6ff;
}

.project-box p {
    padding: 0 1rem 1rem;
    color: #bbb;
}

.project-box .btn {
    margin-bottom: 1rem;
}

.project-box:hover {
    transform: translateY(-8px);
    box-shadow: 0 8px 25px rgba(0,0,0,0.6);
}
.contact {
    padding: 50px 20px;
    background-color: inherit; 
    color: inherit;
    text-align: center;
    border-top: 2px solid #ccc;
}

.contact h2 {
    font-size: 2rem;
    margin-bottom: 20px;
    color: inherit; }

.contact form {
    max-width: 500px;
    margin: 0 auto;
}

.contact input,
.contact textarea {
    width: 100%;
    padding: 12px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 8px;
    font-size: 1rem;
}

.contact button {
    padding: 12px 20px;
    background-color: #3498db; 
    color: #fff;
    border: none;
    border-radius: 8px;
    font-size: 1rem;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.contact button:hover {
    background-color: #2980b9; 
}
```

## OUTPUT
<img width="1897" height="861" alt="Screenshot 2025-08-10 232003" src="https://github.com/user-attachments/assets/55cb59af-7a7d-413e-8d3a-92c3e9e4814f" />
<img width="1890" height="1029" alt="Screenshot 2025-08-10 232018" src="https://github.com/user-attachments/assets/2626d2be-4a91-47dc-8946-b736c1b05a06" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
