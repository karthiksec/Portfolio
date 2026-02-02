# Ex01 Portfolio
## Date:02.02.2026

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
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f4f4;
        }

        header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2rem 0;
            position: sticky;
            top: 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1000px;
            margin: 0 auto;
            padding: 0 20px;
        }

        nav h1 {
            font-size: 1.8rem;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
        }

        nav a:hover {
            opacity: 0.8;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 0 20px;
        }

        section {
            background: white;
            margin: 2rem 0;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        section h2 {
            color: #667eea;
            margin-bottom: 1.5rem;
            font-size: 2rem;
        }

        .hero {
            text-align: center;
            padding: 4rem 2rem;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border-radius: 8px;
            margin: 2rem 0;
        }

        .hero h2 {
            color: white;
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background: white;
            color: #667eea;
            padding: 0.8rem 2rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .project-card {
            background: #f9f9f9;
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 4px solid #667eea;
            transition: transform 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
        }

        .project-card h3 {
            color: #667eea;
            margin-bottom: 0.5rem;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .skill-tag {
            background: #667eea;
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 3rem;
        }

        footer a {
            color: #667eea;
            text-decoration: none;
        }

        footer a:hover {
            text-decoration: underline;
        }

        @media (max-width: 600px) {
            nav ul {
                gap: 1rem;
                font-size: 0.9rem;
            }

            .hero h2 {
                font-size: 2rem;
            }

            section {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <h1>Karthik G</h1>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <div class="container">
        <section id="home" class="hero">
            <h2>Front End Developer</h2>
            <p>Creating beautiful and functional web experiences</p>
            <a href="#projects" class="btn">View My Work</a>
        </section>

        <section id="about">
            <h2>About Me</h2>
            <p>I'm a passionate developer with expertise in building modern web applications. I love turning ideas into reality using the latest technologies and best practices.</p>
            <p style="margin-top: 1rem;">With experience in frontend and backend development, I create full-stack solutions that are scalable, maintainable, and user-friendly.</p>
        </section>

        <section id="projects">
            <h2>My Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <h3>Real Time Website Traffic Visualizer</h3>
                    <p>An interactive visualization tool that displays real-time website traffic data with dynamic charts and analytics. Features live updates, visitor tracking, and comprehensive traffic insights.</p>
                    <div class="skills">
                        <span class="skill-tag">React</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">D3.js</span>
                        <span class="skill-tag">APIs</span>
                    </div>
                </div>
            </div>
        </section>

        <section>
            <h2>Skills</h2>
            <div class="skills">
                <span class="skill-tag">HTML/CSS</span>
                <span class="skill-tag">JavaScript</span>
                <span class="skill-tag">React</span>
                <span class="skill-tag">python</span>
                <span class="skill-tag">java</span>
            </div>
        </section>

        <section id="contact">
            <h2>Get In Touch</h2>
            <p>I'm always interested in hearing about new projects and opportunities. Feel free to reach out!</p>
            <div style="margin-top: 1.5rem;">
                <p><strong>Email:</strong> karthikkarthik152006@gmail.com</p>
                <p><strong>Phone:</strong> 9715331880</p>
                <p style="margin-top: 1rem;">
                    <a href="https://linkedin.com" style="color: #667eea; text-decoration: none; margin-right: 1rem;">LinkedIn</a>
                    <a href="https://github.com" style="color: #667eea; text-decoration: none; margin-right: 1rem;">GitHub</a>
                </p>
            </div>
        </section>
    </div>

    <footer>
        <p>&copy; 2026 Karthik G. All rights reserved. | <a href="#home">Back to top</a></p>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
</body>
</html>

```

## OUTPUT
<img width="1918" height="1079" alt="Screenshot 2026-02-02 102542" src="https://github.com/user-attachments/assets/f66c78c4-cc07-4daf-9fb3-e0a1fdb84458" />

<img width="1919" height="1009" alt="Screenshot 2026-02-02 102550" src="https://github.com/user-attachments/assets/f86e0860-1399-48e2-bf11-705d83bfcda9" />

<img width="1919" height="1079" alt="Screenshot 2026-02-02 102558" src="https://github.com/user-attachments/assets/0ca38f48-2bfc-4869-8701-b7957c0db630" />

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
