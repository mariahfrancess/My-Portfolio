<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Mariah Ballucanag | IT Student Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f7f9fc;
            color: #1e293b;
            line-height: 1.6;
        }

        /* NAVIGATION */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255,255,255,0.95);
            box-shadow: 0 2px 10px rgba(0,0,0,0.08);
            z-index: 1000;
        }

        nav {
            max-width: 1100px;
            margin: auto;
            padding: 18px 25px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #2563eb;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        nav a {
            text-decoration: none;
            color: #334155;
            font-weight: 500;
            transition: 0.3s;
        }

        nav a:hover {
            color: #2563eb;
        }

        /* HERO */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: 100px 25px 50px;
            background: linear-gradient(135deg, #eff6ff, #ffffff);
        }

        .hero-container {
            max-width: 1100px;
            width: 100%;
            margin: auto;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 50px;
        }

        .hero-text {
            flex: 1;
        }

        .hero-text p:first-child {
            color: #2563eb;
            font-weight: bold;
            font-size: 18px;
        }

        .hero h1 {
            font-size: 55px;
            line-height: 1.1;
            margin: 10px 0;
        }

        .hero h1 span {
            color: #2563eb;
        }

        .hero-description {
            max-width: 600px;
            color: #64748b;
            margin: 20px 0;
            font-size: 18px;
        }

        .buttons {
            display: flex;
            gap: 15px;
            margin-top: 25px;
        }

        .btn {
            padding: 12px 25px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        .primary-btn {
            background: #2563eb;
            color: white;
        }

        .primary-btn:hover {
            background: #1d4ed8;
        }

        .secondary-btn {
            border: 2px solid #2563eb;
            color: #2563eb;
        }

        .secondary-btn:hover {
            background: #2563eb;
            color: white;
        }

        .profile-picture {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: #dbeafe;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 80px;
            color: #2563eb;
            border: 8px solid white;
            box-shadow: 0 10px 30px rgba(37,99,235,0.2);
        }

        /* GENERAL SECTION */
        section {
            padding: 90px 25px;
        }

        .section-container {
            max-width: 1100px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .section-title p {
            color: #64748b;
        }

        /* ABOUT */
        .about-content {
            display: flex;
            gap: 50px;
            align-items: center;
        }

        .about-text {
            flex: 1;
        }

        .about-text p {
            margin-bottom: 15px;
            color: #64748b;
        }

        .about-info {
            flex: 1;
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.07);
        }

        .info-item {
            margin-bottom: 18px;
        }

        .info-item strong {
            color: #2563eb;
        }

        /* SKILLS */
        #skills {
            background: #eff6ff;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .skill-card {
            background: white;
            padding: 25px;
            text-align: center;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.06);
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-5px);
        }

        .skill-icon {
            font-size: 35px;
            margin-bottom: 10px;
        }

        .skill-card h3 {
            margin-bottom: 5px;
        }

        .skill-card p {
            color: #64748b;
            font-size: 14px;
        }

        /* PROJECTS */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .project-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.07);
            transition: 0.3s;
        }

        .project-card:hover {
            transform: translateY(-7px);
        }

        .project-image {
            height: 280px;
            background: linear-gradient(135deg, #2563eb, #60a5fa);
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 45px;
        }

        .project-content {
            padding: 25px;
        }

        .project-content h3 {
            margin-bottom: 10px;
        }

        .project-content p {
            color: #64748b;
            font-size: 14px;
            margin-bottom: 15px;
        }

        .project-link {
            color: #2563eb;
            text-decoration: none;
            font-weight: bold;
        }

        /* EDUCATION */
        #education {
            background: #eff6ff;
        }

        .education-card {
            background: white;
            padding: 30px;
            border-left: 5px solid #2563eb;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.06);
            margin-bottom: 20px;
        }

        .education-card h3 {
            color: #2563eb;
        }

        .education-card p {
            color: #64748b;
        }

        /* CONTACT */
        .contact-container {
            max-width: 700px;
            margin: auto;
            text-align: center;
        }

        .contact-container p {
            color: #64748b;
            margin-bottom: 25px;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .contact-link {
            padding: 12px 20px;
            border-radius: 8px;
            background: #eff6ff;
            color: #2563eb;
            text-decoration: none;
            font-weight: bold;
        }

        /* FOOTER */
        footer {
            background: #0f172a;
            color: white;
            text-align: center;
            padding: 25px;
        }

        footer p {
            font-size: 14px;
            color: #cbd5e1;
        }

        /* RESPONSIVE */
        @media (max-width: 800px) {

            nav ul {
                gap: 12px;
                font-size: 14px;
            }

            .hero-container {
                flex-direction: column-reverse;
                text-align: center;
            }

            .hero h1 {
                font-size: 40px;
            }

            .buttons {
                justify-content: center;
            }

            .about-content {
                flex-direction: column;
            }

            .skills-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 500px) {

            nav {
                flex-direction: column;
                gap: 10px;
            }

            nav ul {
                flex-wrap: wrap;
                justify-content: center;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }

            .profile-picture {
                width: 220px;
                height: 220px;
            }
        }
    </style>
</head>

<body>

    <!-- NAVIGATION -->
    <header>
        <nav>
            <div class="logo">MB</div>

            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#education">Education</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>


    <!-- HOME -->
    <section class="hero" id="home">

        <div class="hero-container">

            <div class="hero-text">

                <p>Hello, I'm</p>

                <h1>
                    Mariah <span>Ballucanag</span>
                </h1>

                <p class="hero-description">
                    A Bachelor of Science in Information Technology student
                    specializing in Web and Mobile Application Development.
                    I am passionate about learning technology and creating
                    useful digital solutions.
                </p>

                <div class="buttons">
                    <a href="#projects" class="btn primary-btn">
                        View My Projects
                    </a>

                    <a href="#contact" class="btn secondary-btn">
                        Contact Me
                    </a>
                </div>

            </div>

            <div class="profile-piure">
                <img src="c:\Users\mariah\Downloads\Mariah.jpg" alt="Mariah.jpg" style="width: 200px; height: 300; border-radius: 50%;">

        </div>

    </section>


    <!-- ABOUT -->
    <section id="about">

        <div class="section-container">

            <div class="section-title">
                <h2>About Me</h2>
                <p>Get to know me</p>
            </div>

            <div class="about-content">

                <div class="about-text">

                    <p>
                        I am an Information Technology student who enjoys
                        learning about web and mobile application development.
                    </p>

                    <p>
                        I am currently developing my skills in programming,
                        database management, web development, and software
                        design.
                    </p>

                    <p>
                        My goal is to become a skilled IT professional and
                        create technology-based solutions that can help
                        individuals and organizations.
                    </p>

                </div>

                <div class="about-info">

                    <div class="info-item">
                        <strong>Name:</strong>
                        <p>Mariah Frances Ballucanag</p>
                    </div>

                    <div class="info-item">
                        <strong>Course:</strong>
                        <p>BS Information Technology</p>
                    </div>

                    <div class="info-item">
                        <strong>Specialization:</strong>
                        <p>Web and Mobile Application Development</p>
                    </div>

                    <div class="info-item">
                        <strong>University:</strong>
                        <p>Nueva Vizcaya State University</p>
                    </div>

                </div>

            </div>

        </div>

    </section>


    <!-- SKILLS -->
    <section id="skills">

        <div class="section-container">

            <div class="section-title">
                <h2>My Skills</h2>
                <p>Technologies and skills I am learning</p>
            </div>

            <div class="skills-grid">

                <div class="skill-card">
                    <div class="skill-icon">💻</div>
                    <h3>HTML</h3>
                    <p>Creating website structures</p>
                </div>

                <div class="skill-card">
                    <div class="skill-icon">🎨</div>
                    <h3>CSS</h3>
                    <p>Designing responsive interfaces</p>
                </div>

                <div class="skill-card">
                    <div class="skill-icon">⚡</div>
                    <h3>JavaScript</h3>
                    <p>Adding website functionality</p>
                </div>

                <div class="skill-card">
                    <div class="skill-icon">📱</div>
                    <h3>MIT App Inventor</h3>
                    <p>Building mobile applications</p>
                </div>
            
            </div>

        </div>

    </section>


    <!-- PROJECTS -->
    <section id="projects">

        <div class="section-container">

            <div class="section-title">
                <h2>My Projects</h2>
                <p>Some of my school and personal projects</p>
            </div>

            <div class="projects-grid">

                <div class="project-card">


                    <div class="project-content">

                        <h3>Bean-There-Coffee-Shop</h3>

                        <p>
                            A sleek, engaging front-end web page developed to showcase the brand, menu, ambiance of a cozy coffee shop in a clean and visually appealing layout.
                        </p>

                        <a href="#" class="project-link">
                            View Project →
                        </a>

                    </div>

                </div>


                <div class="project-card">


                    <div class="project-content">

                        <h3>Cel-Kal-Culator</h3>

                        <p>
                            A mobile temperature converter created using
                            MIT App Inventor that converts Celsius into
                            Fahrenheit and Kelvin.
                        </p>

                        <a href="#" class="project-link">
                            View Project →
                        </a>

                    </div>

                </div>

        </div>

    </section>


    <!-- EDUCATION -->
    <section id="education">

        <div class="section-container">

            <div class="section-title">
                <h2>Education</h2>
                <p>My academic journey</p>
            </div>

            <div class="education-card">

                <h3>Bachelor of Science in Information Technology</h3>

                <p>
                    Web and Mobile Application Development
                </p>

                <p>
                    Nueva Vizcaya State University
                </p>

                <p>
                    Present
                </p>

            </div>

            <div class="education-card">

                <h3>Senior High School – STEM</h3>

                <p>
                    Bintawan National High School
                </p>

            </div>

        </div>

    </section>


    <!-- CONTACT -->
    <section id="contact">

        <div class="section-container">

            <div class="section-title">
                <h2>Let's Connect</h2>
                <p>Feel free to reach out to me</p>
            </div>

            <div class="contact-container">

                <p>
                    I am always open to learning, collaborating, and
                    connecting with other people interested in technology.
                </p>

                <div class="contact-links">

                    <a href="mariahfrancessb@gmail.com" class="contact-link">
                        📧 Email
                    </a>

                    <a href="https://www.facebook.com/share/1ByiweY3cc/?mibextid=wwXIfr" class="contact-link">
                        📘 Facebook
                    </a>


                </div>

            </div>

        </div>

    </section>


    <!-- FOOTER -->
    <footer>

        <p>
            © 2026 Mariah Ballucanag. All Rights Reserved.
        </p>

        <p>
            Built with HTML & CSS
        </p>

    </footer>


</body>
</html>, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
