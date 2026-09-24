import os

# Define directory structure and complete file contents
files = {
    "index.html": """<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Okikiola Hassan Arowoshola | Home</title>
  <link rel="stylesheet" href="css/styles.css">
</head>
<body>

  <header>
    <nav class="navbar">
      <div class="logo">Okikiola<span>.dev</span></div>
      <ul class="nav-links">
        <li><a href="index.html" class="active">Home</a></li>
        <li><a href="about.html">About Me</a></li>
        <li><a href="projects.html">Projects</a></li>
        <li><a href="planner.html">Academic Planner</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <section class="hero-section">
      <div class="hero-image">
        <img src="https://via.placeholder.com/200" alt="Okikiola Hassan Arowoshola">
      </div>
      <div class="hero-text">
        <h1>Welcome to My Academic Portfolio! 👋</h1>
        <h2>Okikiola Hassan Arowoshola</h2>
        <p class="tagline">Computer Science Student & Web Developer in Training</p>
        <p class="bio">
          Hello! I am a student pursuing my studies in Web Technologies and Computer Science.
          This website serves as my academic portfolio and management system, showcasing my skills, 
          projects, and dynamic tools built for student productivity.
        </p>
        <div class="cta-buttons">
          <a href="projects.html" class="btn primary-btn">View My Projects</a>
          <a href="contact.html" class="btn secondary-btn">Get In Touch</a>
        </div>
      </div>
    </section>

    <section class="multimedia-section">
      <h3>Audio Introduction</h3>
      <audio controls>
        <source src="https://www.w3schools.com/html/horse.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </section>
  </main>

  <footer>
    <p>&copy; 2026 Okikiola Hassan Arowoshola | COS 106 Term Project. All Rights Reserved.</p>
  </footer>

</body>
</html>""",

    "about.html": """<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Me | Okikiola Hassan Arowoshola</title>
  <link rel="stylesheet" href="css/styles.css">
</head>
<body>

  <header>
    <nav class="navbar">
      <div class="logo">Okikiola<span>.dev</span></div>
      <ul class="nav-links">
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html" class="active">About Me</a></li>
        <li><a href="projects.html">Projects</a></li>
        <li><a href="planner.html">Academic Planner</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <h1>About Me</h1>

    <section class="about-card">
      <h2>🎓 Educational Background</h2>
      <p>Currently studying Computer Science, focusing on Web Technologies, Software Engineering, and Database Management Systems.</p>
    </section>

    <section class="about-card">
      <h2>🎯 Career Aspirations</h2>
      <p>My goal is to become a Full-Stack Software Engineer building cloud-native, scalable, and responsive user experiences.</p>
    </section>

    <section class="about-card">
      <h2>💻 Technical Skills</h2>
      <table class="skills-table">
        <thead>
          <tr>
            <th>Category</th>
            <th>Technologies</th>
            <th>Proficiency</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Frontend</td>
            <td>HTML5, CSS3, JavaScript (ES6+)</td>
            <td>Intermediate</td>
          </tr>
          <tr>
            <td>Version Control</td>
            <td>Git, GitHub</td>
            <td>Intermediate</td>
          </tr>
          <tr>
            <td>Layouts</td>
            <td>Flexbox, CSS Grid, Responsive Design</td>
            <td>Advanced</td>
          </tr>
        </tbody>
      </table>
    </section>

    <section class="about-card">
      <h2>🎨 Hobbies and Interests</h2>
      <ul>
        <li>Building creative web applications</li>
        <li>Solving coding challenges</li>
        <li>Reading technology blogs</li>
        <li>Playing strategic board games</li>
      </ul>
    </section>
  </main>

  <footer>
    <p>&copy; 2026 Okikiola Hassan Arowoshola | COS 106 Term Project</p>
  </footer>

</body>
</html>""",

    "projects.html": """<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Projects | Okikiola Hassan Arowoshola</title>
  <link rel="stylesheet" href="css/styles.css">
</head>
<body>

  <header>
    <nav class="navbar">
      <div class="logo">Okikiola<span>.dev</span></div>
      <ul class="nav-links">
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About Me</a></li>
        <li><a href="projects.html" class="active">Projects</a></li>
        <li><a href="planner.html">Academic Planner</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <h1>My Academic Projects</h1>
    <p class="subtitle">A showcase of practical projects completed during my studies.</p>

    <div class="projects-grid">
      <article class="project-card">
        <img src="https://via.placeholder.com/350x200?text=Student+Portfolio" alt="Student Portfolio">
        <h3>1. Student Portfolio Website</h3>
        <p>A multi-page responsive web project for COS 106 featuring dynamic navigation, embedded media, and CSS flexbox styling.</p>
        <p><strong>Tech Stack:</strong> HTML5, CSS3, JS</p>
        <a href="index.html" class="btn primary-btn">View Home</a>
      </article>

      <article class="project-card">
        <img src="https://via.placeholder.com/350x200?text=Academic+Planner" alt="Academic Planner">
        <h3>2. Academic Task Planner</h3>
        <p>An interactive JavaScript web utility that allows students to add, mark complete, and delete personal academic tasks.</p>
        <p><strong>Tech Stack:</strong> JavaScript DOM, CSS</p>
        <a href="planner.html" class="btn primary-btn">Try Demo</a>
      </article>

      <article class="project-card">
        <img src="https://via.placeholder.com/350x200?text=Contact+Validator" alt="Form Validator">
        <h3>3. Client-Side Form Validator</h3>
        <p>A custom form validation script ensuring correct input handling, email regex checks, and numeric phone verification.</p>
        <p><strong>Tech Stack:</strong> HTML Forms, JS Regex</p>
        <a href="contact.html" class="btn primary-btn">Test Form</a>
      </article>
    </div>
  </main>

  <footer>
    <p>&copy; 2026 Okikiola Hassan Arowoshola | COS 106 Term Project</p>
  </footer>

</body>
</html>""",

    "planner.html": """<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Academic Planner | Okikiola Hassan Arowoshola</title>
  <link rel="stylesheet" href="css/styles.css">
</head>
<body>

  <header>
    <nav class="navbar">
      <div class="logo">Okikiola<span>.dev</span></div>
      <ul class="nav-links">
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About Me</a></li>
        <li><a href="projects.html">Projects</a></li>
        <li><a href="planner.html" class="active">Academic Planner</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <h1>Interactive Academic Planner</h1>
    <p class="subtitle">Manage your study tasks, coursework, and deadlines.</p>

    <div class="planner-wrapper">
      <form id="planner-form">
        <input type="text" id="task-input" placeholder="Enter task (e.g., Submit COS 106 Project)...">
        <button type="submit" class="btn primary-btn">Add Task</button>
      </form>

      <ul id="task-list" class="task-list"></ul>
    </div>
  </main>

  <footer>
    <p>&copy; 2026 Okikiola Hassan Arowoshola | COS 106 Term Project</p>
  </footer>

  <script src="js/script.js"></script>
</body>
</html>""",

    "contact.html": """<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact | Okikiola Hassan Arowoshola</title>
  <link rel="stylesheet" href="css/styles.css">
</head>
<body>

  <header>
    <nav class="navbar">
      <div class="logo">Okikiola<span>.dev</span></div>
      <ul class="nav-links">
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About Me</a></li>
        <li><a href="projects.html">Projects</a></li>
        <li><a href="planner.html">Academic Planner</a></li>
        <li><a href="contact.html" class="active">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <h1>Contact Me</h1>
    <p class="subtitle">Fill in the form below to send a message.</p>

    <div class="contact-wrapper">
      <div id="error-message" class="alert-box error" style="display: none;"></div>
      <div id="success-message" class="alert-box success" style="display: none;"></div>

      <form id="contact-form" novalidate>
        <div class="form-group">
          <label for="fullname">Full Name *</label>
          <input type="text" id="fullname" name="fullname" placeholder="Okikiola Arowoshola">
        </div>

        <div class="form-group">
          <label for="email">Email Address *</label>
          <input type="email" id="email" name="email" placeholder="example@mail.com">
        </div>

        <div class="form-group">
          <label for="phone">Phone Number *</label>
          <input type="tel" id="phone" name="phone" placeholder="08012345678">
        </div>

        <div class="form-group">
          <label for="message">Message *</label>
          <textarea id="message" name="message" rows="5" placeholder="Write your message..."></textarea>
        </div>

        <button type="submit" class="btn primary-btn">Send Message</button>
      </form>
    </div>
  </main>

  <footer>
    <p>&copy; 2026 Okikiola Hassan Arowoshola | COS 106 Term Project</p>
  </footer>

  <script src="js/script.js"></script>
</body>
</html>""",

    "css/styles.css": """* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  background-color: #f4f6f9;
  color: #333;
}

header {
  background-color: #1e293b;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1100px;
  margin: 0 auto;
  padding: 1rem 2rem;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  color: #ffffff;
}

.logo span {
  color: #38bdf8;
}

.nav-links {
  display: flex;
  list-style: none;
  gap: 1.5rem;
}

.nav-links a {
  color: #cbd5e1;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
}

.nav-links a:hover, .nav-links a.active {
  color: #38bdf8;
  border-bottom: 2px solid #38bdf8;
}

.container {
  max-width: 1100px;
  margin: 2rem auto;
  padding: 0 1.5rem;
  min-height: 80vh;
}

.subtitle {
  margin-bottom: 2rem;
  color: #64748b;
}

.hero-section {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 2rem;
  background-color: #ffffff;
  padding: 2.5rem;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
}

.hero-image img {
  border-radius: 50%;
  border: 4px solid #38bdf8;
}

.hero-text {
  flex: 1;
}

.tagline {
  color: #2563eb;
  font-weight: bold;
  margin-bottom: 1rem;
}

.btn {
  display: inline-block;
  padding: 0.7rem 1.4rem;
  border-radius: 5px;
  text-decoration: none;
  font-weight: 600;
  cursor: pointer;
  border: none;
  transition: transform 0.2s ease;
}

.btn:hover {
  transform: translateY(-2px);
}

.primary-btn {
  background-color: #2563eb;
  color: white;
}

.secondary-btn {
  background-color: #e2e8f0;
  color: #1e293b;
  margin-left: 0.5rem;
}

.multimedia-section {
  margin-top: 2rem;
  background: white;
  padding: 1.5rem;
  border-radius: 8px;
}

.skills-table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 1rem;
}

.skills-table th, .skills-table td {
  border: 1px solid #cbd5e1;
  padding: 0.75rem;
  text-align: left;
}

.skills-table th {
  background-color: #f1f5f9;
}

.about-card {
  background: white;
  padding: 1.5rem;
  border-radius: 8px;
  margin-bottom: 1.5rem;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
}

.project-card {
  background: white;
  padding: 1.5rem;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
}

.project-card img {
  width: 100%;
  border-radius: 5px;
  margin-bottom: 1rem;
}

.planner-wrapper, .contact-wrapper {
  background: white;
  padding: 2rem;
  border-radius: 8px;
}

#planner-form {
  display: flex;
  gap: 1rem;
  margin-bottom: 1.5rem;
}

#task-input {
  flex: 1;
  padding: 0.75rem;
  border: 1px solid #cbd5e1;
  border-radius: 5px;
}

.task-list {
  list-style: none;
}

.task-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.75rem 1rem;
  background: #f8fafc;
  border: 1px solid #e2e8f0;
  border-radius: 5px;
  margin-bottom: 0.5rem;
}

.task-item.completed span {
  text-decoration: line-through;
  color: #94a3b8;
}

.delete-btn {
  background: #ef4444;
  color: white;
  border: none;
  padding: 0.4rem 0.8rem;
  border-radius: 4px;
  cursor: pointer;
}

.form-group {
  margin-bottom: 1.2rem;
}

.form-group label {
  display: block;
  margin-bottom: 0.4rem;
  font-weight: 600;
}

.form-group input, .form-group textarea {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid #cbd5e1;
  border-radius: 5px;
}

.alert-box {
  padding: 1rem;
  border-radius: 5px;
  margin-bottom: 1rem;
}

.alert-box.error {
  background-color: #fef2f2;
  color: #dc2626;
  border: 1px solid #fecaca;
}

.alert-box.success {
  background-color: #f0fdf4;
  color: #16a34a;
  border: 1px solid #bbf7d0;
}

footer {
  text-align: center;
  padding: 1.5rem;
  background-color: #0f172a;
  color: #94a3b8;
  margin-top: 3rem;
}

@media (max-width: 768px) {
  .navbar { flex-direction: column; gap: 1rem; }
  .nav-links { flex-wrap: wrap; justify-content: center; }
  #planner-form { flex-direction: column; }
}""",

    "js/script.js": """document.addEventListener("DOMContentLoaded", () => {
  
  // Task Planner Logic
  const plannerForm = document.getElementById("planner-form");
  const taskInput = document.getElementById("task-input");
  const taskList = document.getElementById("task-list");

  let tasks = [];

  if (plannerForm) {
    plannerForm.addEventListener("submit", (e) => {
      e.preventDefault();
      const taskText = taskInput.value.trim();

      if (taskText !== "") {
        tasks.push({ id: Date.now(), text: taskText, completed: false });
        taskInput.value = "";
        renderTasks();
      }
    });
  }

  function renderTasks() {
    if (!taskList) return;
    taskList.innerHTML = "";

    tasks.forEach(task => {
      const li = document.createElement("li");
      li.className = `task-item ${task.completed ? "completed" : ""}`;

      const span = document.createElement("span");
      span.textContent = task.text;
      span.addEventListener("click", () => {
        task.completed = !task.completed;
        renderTasks();
      });

      const delBtn = document.createElement("button");
      delBtn.className = "delete-btn";
      delBtn.textContent = "Delete";
      delBtn.addEventListener("click", () => {
        tasks = tasks.filter(t => t.id !== task.id);
        renderTasks();
      });

      li.appendChild(span);
      li.appendChild(delBtn);
      taskList.appendChild(li);
    });
  }

  // Form Validation Logic
  const contactForm = document.getElementById("contact-form");
  const errorMessage = document.getElementById("error-message");
  const successMessage = document.getElementById("success-message");

  if (contactForm) {
    contactForm.addEventListener("submit", (e) => {
      e.preventDefault();

      errorMessage.style.display = "none";
      successMessage.style.display = "none";

      const fullName = document.getElementById("fullname").value.trim();
      const email = document.getElementById("email").value.trim();
      const phone = document.getElementById("phone").value.trim();
      const message = document.getElementById("message").value.trim();

      let errors = [];

      if (!fullName || !email || !phone || !message) {
        errors.push("All fields are required.");
      }

      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      if (email && !emailRegex.test(email)) {
        errors.push("Please enter a valid email address.");
      }

      const phoneRegex = /^\d+$/;
      if (phone && !phoneRegex.test(phone)) {
        errors.push("Phone number must contain only digits.");
      }

      if (errors.length > 0) {
        errorMessage.innerHTML = errors.join("<br>");
        errorMessage.style.display = "block";
      } else {
        successMessage.textContent = "Message sent successfully!";
        successMessage.style.display = "block";
        contactForm.reset();
      }
    });
  }
});""",

    "README.md": """# Okikiola Hassan Arowoshola - Student Portfolio

Responsive multi-page academic portfolio and student management website for **COS 106 - Introduction to Web Technologies**.

## Included Pages
* `index.html`: Student introduction and media section.
* `about.html`: Educational background, career goals, technical skills table, and interests.
* `projects.html`: Portfolio of practical project highlights.
* `planner.html`: Interactive task planner built with JavaScript DOM manipulation.
* `contact.html`: Contact form with JavaScript validation (non-empty fields, valid email format, digit-only phone number).

## Author
* **Name:** Okikiola Hassan Arowoshola
* **Course:** COS 106 - Introduction to Web Technologies"""
}

# Create subdirectories if they don't exist
os.makedirs("css", exist_ok=True)
os.makedirs("js", exist_ok=True)

# Generate each file
for file_path, content in files.items():
    with open(file_path, "w", encoding="utf-8") as f:
        f.write(content)
    print(f"Created: {file_path}")

print("\nDone! All 8 files have been created in your folder.")
