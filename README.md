Here is the **updated README section**, exactly as you asked —
I added the steps **before Step 1** (Create new Jenkins job → Freestyle project → Save),
and kept everything else the same.

Fully ready to paste into your README.md.

---

# 📘 **README – Portfolio Website Deployment Using Jenkins (Freestyle Project)**

---

# 📂 **Copy this code in your Desktop folder, then create the GitHub repository using the below commands and push it. After that, follow the further Jenkins process.**

---

# 🌐 Portfolio Website Code

---

# 📄 **index.html**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>My Portfolio</title>
<link rel="stylesheet" href="style.css" />
</head>
<body>

<nav>
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
</nav>

<div class="hero">
  <h1>Hi, I'm a Developer</h1>
  <p>I build websites and simple projects.</p>
  <a class="btn" href="about.html">Know More</a>
</div>

<div class="section">
  <h2>My Projects</h2>
  <div class="card">
    <p>★ ★ ★ ★ ★</p>
    <p>Portfolio Website</p>
    <p>To-Do App</p>
    <p>Weather App</p>
  </div>
</div>

</body>
</html>
```

---

# 📄 **about.html**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>About Me</title>
<link rel="stylesheet" href="style.css" />
</head>
<body>

<nav>
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
</nav>

<div class="container">
  <h1>About Me</h1>
  <p>Hello! I'm a web developer who enjoys building clean and simple websites.</p>
  <p>I love front-end development and learning new tools.</p>
  <p style="text-align:center; font-size:28px; color:#e91e63;">
    ★ ★ ★ ★ ★
  </p>
</div>

</body>
</html>
```

---

# 🎨 **style.css**

```css
body{
  margin:0;
  font-family:Arial;
  background:#f4f4f4;
  color:#222;
}

/* Navbar */
nav{
  background:#111;
  padding:15px;
  text-align:center;
}
nav a{
  color:white;
  text-decoration:none;
  margin:15px;
  font-size:18px;
}

/* Home Hero Section */
.hero{
  height:70vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
  background:#2c3e50;
  color:white;
}
.hero h1{
  font-size:48px;
  margin:0;
}
.hero p{
  font-size:20px;
  margin:10px 0;
}
.btn{
  background:#e91e63;
  color:white;
  padding:10px 20px;
  border-radius:5px;
  text-decoration:none;
  margin-top:15px;
  display:inline-block;
}

/* Common Section */
.section{
  padding:40px;
  text-align:center;
}
.card{
  max-width:600px;
  margin:auto;
  background:white;
  padding:20px;
  border-radius:10px;
  box-shadow:0 4px 10px rgba(0,0,0,0.1);
}

/* About Page */
.container{
  max-width:700px;
  margin:50px auto;
  background:white;
  padding:30px;
  border-radius:10px;
  box-shadow:0 4px 10px rgba(0,0,0,0.2);
}
h1{
  color:#333;
  text-align:center;
}
p{
  line-height:1.6;
  font-size:18px;
}
```

---

# 📝 Git Commands

Use the following commands to initialize Git and push your project to GitHub:

```bash
git init
git add .
git commit -m "First portfolio commit"
git branch -M main
git remote add origin https://github.com/your-username/portfolio.git
git push -u origin main
```

---

# ⚙️ Jenkins Freestyle Project – Build Periodically Setup

### **Before Step 1: Create the Jenkins Job**

**Step A:** Click on **New Item**

**Step B:** Enter the project name

**Step C:** Select **Freestyle Project**

**Step D:** Click **Save**

---

### **Build Periodically Process**

**Step 1:**
Click on **Build periodically** in the **Build Triggers** section.

**Step 2:**
In **Build periodically → Schedule**, add 5 stars with spaces:

```
* * * * *
```

**Step 3:**
Click **Save**.

**Step 4:**
Click **Build Now**.

**Step 5:**
The job will start building **every minute**.
To stop it:
Go to **Configure → uncheck Build periodically → Save**.

---
