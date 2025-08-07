<!-- Banner -->
<!-- Banner -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Profile Banner</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #0f172a;
        }
        
        .banner-container {
            height: 500px;
            width: 1500px;
            position: relative;
            overflow: hidden;
            border-radius: 12px;
        }
        
        .tech-decoration {
            position: absolute;
            color: rgba(255, 255, 255, 0.1);
            font-size: 24px;
            font-weight: bold;
        }
        
        .profile-badge {
            position: absolute;
            bottom: 40px;
            right: 40px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 8px;
            padding: 16px 24px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
    </style>
</head>
<body class="flex items-center justify-center min-h-screen">
    <div class="banner-container bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500">
        <!-- Background image placeholder (will be automatically generated from alt text) -->
        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/75ff77e4-3a6d-47e0-a6d3-530bc7a27a40.png" alt="Professional banner featuring dark blue background with modern tech elements and developer name" class="absolute inset-0 w-full h-full object-cover" />
        
        <!-- Tech decoration elements -->
        <div class="tech-decoration left-20 top-20 transform rotate-12">{ }</div>
        <div class="tech-decoration right-40 top-32 transform -rotate-6">console.log()</div>
        <div class="tech-decoration left-64 bottom-40 transform rotate-45"><div></div>
        <div class="tech-decoration right-80 bottom-24 transform -rotate-12">npm start</div>
        
        <!-- Main content -->
        <div class="absolute inset-0 flex flex-col justify-center pl-20">
            <h1 class="text-white text-6xl font-extrabold mb-4 drop-shadow-lg">
                MD JAKARIA
                <span class="text-yellow-300">MERN STACK DEVELOPER</span>
            </h1>
            <p class="text-xl text-white/80 max-w-lg">
                Full-Stack Developer | Open Source Contributor
                <span id="typed" class="block text-yellow-300 text-2xl mt-2 font-semibold"></span>
            </p>
        </div>
        
        <!-- Profile badge -->
        <div class="profile-badge">
            <div class="flex items-center gap-3">
                <div class="w-12 h-12 rounded-full overflow-hidden border-2 border-white">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/201f3d35-d198-4315-8e4e-85c9d0c01832.png" alt="Profile initial badge with dark blue background" class="w-full h-full object-cover" />
                </div>
                <div>
                    <h3 class="text-white font-bold">@jakariahossain12</h3>
                    <p class="text-white/80 text-sm">Profile Last Updated: <span id="current-date"></span></p>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Typing animation for skills
        const typedText = document.getElementById('typed');
        const skills = ['JavaScript', 'React', 'Node.js', 'MongoDB', 'Express.js', 'Next.js'];
        let skillIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        let typingSpeed = 100;
        
        function typeWriter() {
            const currentSkill = skills[skillIndex];
            
            if (isDeleting) {
                typedText.textContent = currentSkill.substring(0, charIndex - 1);
                charIndex--;
                typingSpeed = 50;
            } else {
                typedText.textContent = currentSkill.substring(0, charIndex + 1);
                charIndex++;
                typingSpeed = 100;
            }
            
            if (!isDeleting && charIndex === currentSkill.length) {
                isDeleting = true;
                typingSpeed = 1500; // Pause at end of word
            } else if (isDeleting && charIndex === 0) {
                isDeleting = false;
                skillIndex = (skillIndex + 1) % skills.length;
                typingSpeed = 500; // Pause before typing next word
            }
            
            setTimeout(typeWriter, typingSpeed);
        }
        
        // Display current date
        const currentDate = new Date();
        const options = { year: 'numeric', month: 'long', day: 'numeric' };
        document.getElementById('current-date').textContent = currentDate.toLocaleDateString('en-US', options);
        
        // Start animation
        setTimeout(typeWriter, 1000);
    </script>
</body>
</html>


<h1 align="center">Hi 👋, I'm Md Jakaria</h1>
<h3 align="center">MERN Stack Developer based in Kuwait</h3>

---

### 🧑‍💻 About Me

I’m a passionate and self-motivated **MERN Stack Developer** with a strong focus on creating efficient, scalable, and user-friendly web applications. I enjoy solving real-world problems through full-stack projects and always strive to learn new technologies.

I'm open to new opportunities, collaborations, and freelance projects. Let's connect and build something amazing together!

---

### 🔭 Current Activities

- 🚀 Exploring advanced **Next.js** features
- 🔧 Building a **door-to-door parcel delivery platform**
- 🧠 Improving backend skills using **Node.js**, **Express.js**, **MongoDB**, and **Firebase**
- 🎨 Enhancing UI/UX using **Tailwind CSS**


---

### 💼 Skills & Tools

**Main Stack:**  
React · Node.js · Express · MongoDB

**Other Tools:**  
Firebase · Tailwind CSS · Git · VS Code

<p align="center">
  <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,express,mongodb,firebase,tailwind,git,vscode" />
</p>

---

### 🚩 Featured Projects
<!--
- [Parcel Delivery Platform](https://github.com/jakariahossain12/parcel-delivery) – Door-to-door parcel delivery solution.
- [Your Next.js App](https://github.com/jakariahossain12/your-nextjs-app)  -->
<!-- Add or update project links above -->

---


<!-- Add your real certifications, awards, or contributions here -->

---

### 🌐 Connect With Me

<p align="center">
  <a href="mailto:kjakria53@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/md-zakaria-hossain-40b6b6249"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</p>

---

### 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=jakariahossain12&show_icons=true&theme=tokyonight" alt="jakariahossain12 stats" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=jakariahossain12&theme=tokyonight" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=jakariahossain12&layout=compact&theme=tokyonight" />
</p>

---

### 🧠 Fun Fact
> “The best way to learn is to build. I code things that solve real problems.”
