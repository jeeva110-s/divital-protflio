<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resume - jeevanandhini</title>
   
    <!-- CSS Styles -->
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: auto;
            padding: 20px;
            background-color: #f8f9fa;
        }
        .container {
            background: white;
            padding: 20px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
        }
        header {
            text-align: center;
            padding-bottom: 20px;
            border-bottom: 2px solid #ddd;
        }
        .profile-pic {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            display: block;
            margin: 0 auto 10px;
        }
        h1, h2 {
            color: #333;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        li {
            margin-bottom: 8px;
        }
        section {
            margin: 20px 0;
        }
        footer {
            text-align: center;
            padding-top: 10px;
            font-size: 14px;
            color: #666;
        }
        .buttons {
            text-align: center;
            margin-top: 20px;
        }
        button {
            padding: 10px 15px;
            background-color: #007bff;
            color: white;
            border: none;
            cursor: pointer;
            margin: 5px;
            border-radius: 5px;
        }
        button:hover {
            background-color: #0056b3;
        }
        /* Hide buttons when printing */
        @media print {
            .buttons {
                display: none;
            }
        }
    </style>

    <div class="container" id="resume">
        <header>
            <!-- Add the image for profile picture -->
            <img src="C:\Users\jeeva\Downloads\IMG-20250110-WA0148 (1).jpg" alt="Profile Picture" class="profile-pic">
            <h1>jeeva nandhini.S</h1>
            <p>BCA Student | Aspiring App Developer</p>
            <p>Email: jeevanandhini05122005@gmail.com | Phone: 9361851383 | LinkedIn: www.linkedin.com/in/jeevanandhini-895a55291</p>
        </header>

        <section>
            <h2>Professional Summary</h2>
            <p>A highly motivated and detail-oriented BCA student with a strong foundation in computer science, programming, and software development. Proficient in languages like Python, Java, and C++, with hands-on experience in web development and database management.</p>
        </section>

        <section>
            <h2>Projects</h2>
            <ul>
                <li><strong>Portfolio Website:</strong> Built a personal portfolio showcasing projects and achievements using HTML, CSS, and JavaScript.</li>
                <li><strong>Weather App:</strong> Created an application that fetches live weather data using an API.</li>
                <li><strong>To-Do List App:</strong> Developed a to-do list app with local storage functionality.</li>
            </ul>
        </section>

        <section>
            <h2>Education</h2>
            <p><strong>Bachelor of Computer Applications (BCA)</strong><br>Bharathiar University | 2023 - 2026 | Current CGPA: 6.5/10</p>
        </section>

        <section>
            <h2>Skills</h2>
            <ul>
                <li>Programming Languages: C, C++, Python, JavaScript</li>
                <li>Web Development: HTML5, CSS3, JavaScript, React</li>
                <li>Database: MySQL, MongoDB</li>
                <li>Tools: Git, GitHub, VS Code</li>
                <li>Problem Solving, Debugging, Team Collaboration</li>
            </ul>
        </section>

        <section>
            <h2>Certifications</h2>
            <ul>
                <li>HTML, CSS, and JavaScript Certification - freeCodeCamp</li>
                <li>Python for Beginners - Coursera</li>
                <li>Git & GitHub Mastery - Udemy</li>
                <li>Naan Mudhalvan certificates</li>
            </ul>
        </section>

        <section>
            <h2>Languages</h2>
            <ul>
                <li>English (Fluent)</li>
                <li>Tamil (Fluent)</li>
                <li>Badagar (Native)</li>
            </ul>
        </section>

        <footer>
            <p>© 2025 jeeva nandhini | Built with HTML & CSS</p>
        </footer>
    </div>

    <!-- Buttons for PDF Download -->
    <div class="buttons">
        <button onclick="window.print()">Print / Save as PDF</button>
        <button id="download">Download as PDF</button>
    </div>

    <!-- JavaScript for PDF Download -->
    <script>
        document.getElementById("download").addEventListener("click", function () {
            const resume = document.getElementById("resume");
            html2pdf().from(resume).save("jeevanandhini_Resume.pdf");
        });
    </script>
</body>
</html>
