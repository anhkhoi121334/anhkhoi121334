<!-- 3D Particle Background Header -->
<!-- Note: JavaScript animation works in browsers but not in GitHub's markdown preview -->
<div style="position: relative; width: 100%; height: 300px; overflow: hidden; border-radius: 10px; margin-bottom: 2rem; background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);">
  <canvas id="particleCanvas" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></canvas>
  <div style="position: relative; z-index: 2; padding: 2rem; text-align: center; color: white; text-shadow: 0 0 10px rgba(0,0,0,0.5);">
    <h1 style="font-size: 2.5rem; margin-bottom: 0.5rem;">Hi there 👋, I'm Khôi</h1>
    <p style="font-size: 1.5rem; margin-top: 0; opacity: 0.9;">Frontend Developer | React Enthusiast</p>
    <div style="margin-top: 1rem;">
      <a href="https://linkedin.com/in/anhkhoi121334" style="margin: 0 5px;">
        <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
      </a>
      <a href="mailto:khoi21007@gmail.com" style="margin: 0 5px;">
        <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
      </a>
      <a href="https://github.com/anhkhoi121334" style="margin: 0 5px;">
        <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
      </a>
    </div>
    <div style="margin-top: 1rem;">
      <img src="https://komarev.com/ghpvc/?username=anhkhoi121334&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />
    </div>
  </div>
</div>

<script>
// 3D Particle Background
document.addEventListener('DOMContentLoaded', function() {
  const canvas = document.getElementById('particleCanvas');
  const ctx = canvas.getContext('2d');
  let width = canvas.width = canvas.offsetWidth;
  let height = canvas.height = canvas.offsetHeight;
  
  // Handle window resize
  window.addEventListener('resize', function() {
    width = canvas.width = canvas.offsetWidth;
    height = canvas.height = canvas.offsetHeight;
  });

  // Particle system
  const particles = [];
  const particleCount = Math.min(100, Math.floor(width * height / 2000));
  const colors = ['#4facfe', '#00f2fe', '#5ee7df', '#667eea'];

  // Create particles
  for (let i = 0; i < particleCount; i++) {
    particles.push({
      x: Math.random() * width,
      y: Math.random() * height,
      size: Math.random() * 3 + 1,
      color: colors[Math.floor(Math.random() * colors.length)],
      speedX: Math.random() * 2 - 1,
      speedY: Math.random() * 2 - 1
    });
  }

  // Animation loop
  function animate() {
    ctx.clearRect(0, 0, width, height);
    
    // Update and draw particles
    particles.forEach(particle => {
      // Move particles
      particle.x += particle.speedX;
      particle.y += particle.speedY;
      
      // Bounce off edges
      if (particle.x < 0 || particle.x > width) particle.speedX *= -1;
      if (particle.y < 0 || particle.y > height) particle.speedY *= -1;
      
      // Draw particle
      ctx.beginPath();
      ctx.arc(particle.x, particle.y, particle.size, 0, Math.PI * 2);
      ctx.fillStyle = particle.color;
      ctx.fill();
      
      // Draw connections
      particles.forEach(otherParticle => {
        const dx = particle.x - otherParticle.x;
        const dy = particle.y - otherParticle.y;
        const distance = Math.sqrt(dx * dx + dy * dy);
        
        if (distance < 100) {
          ctx.beginPath();
          ctx.strokeStyle = `${particle.color}${Math.round((1 - distance/100) * 0.3 * 255).toString(16).padStart(2, '0')}`;
          ctx.lineWidth = 0.5;
          ctx.moveTo(particle.x, particle.y);
          ctx.lineTo(otherParticle.x, otherParticle.y);
          ctx.stroke();
        }
      });
    });
    
    requestAnimationFrame(animate);
  }
  
  // Start animation
  animate();
});
</script>

<p align="center">
  Sinh viên mới tốt nghiệp với niềm đam mê phát triển giao diện web hiện đại.<br/>
  Chuyên xây dựng các ứng dụng web responsive, tối ưu trải nghiệm người dùng và hiệu suất cao.<br/>
  Luôn tìm tòi và học hỏi những công nghệ mới để nâng cao kỹ năng phát triển.
</p>

<br>

## 🛠️ Tech Stack

### 🚀 Frontend
<div align="left">
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img alt="React" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img alt="Tailwind CSS" src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img alt="Bootstrap" src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" />
</div>

### ⚙️ Backend & Tools
<div align="left">
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img alt="Express" src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img alt="REST API" src="https://img.shields.io/badge/REST_API-FF6C37?style=for-the-badge&logo=postman&logoColor=white" />
  <img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img alt="Git" src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img alt="GitHub" src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />
  <img alt="VS Code" src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" />
</div>

<br>

## 🚀 Featured Projects

### 🛍️ Sneaker Store – E-commerce Website
[![Sneaker Store](https://img.shields.io/badge/View_Live-Demo-2ea44f?style=for-the-badge)](https://elegant-sundae-416b3f.netlify.app/)
[![GitHub](https://img.shields.io/badge/View_Code-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anhkhoi121334/duancanhan2)

A modern e-commerce platform for sneaker enthusiasts with full shopping cart functionality, user authentication, and responsive design.

- **Tech Stack**: ReactJS, TailwindCSS, Zustand, REST API
- **Features**:
  - Product catalog with filtering and search
  - Shopping cart and checkout process
  - User authentication and order history
  - Responsive design for all devices

---

### 💻 E-commerce Electronics Store
[![GitHub FE](https://img.shields.io/badge/Frontend_Repo-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anhkhoi121334/my-phim/tree/master/font-end)
[![GitHub BE](https://img.shields.io/badge/Backend_Repo-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anhkhoi121334/my-phim/tree/master/back-end)

A full-stack e-commerce solution for electronic products with separate frontend and backend architecture.

- **Tech Stack**: ReactJS, TailwindCSS, Zustand, Node.js, Express, MongoDB
- **Features**:
  - Product management system
  - Shopping cart functionality
  - User authentication
  - Order processing system

<br>

## 📊 GitHub Stats

<div align="center">
  <a href="https://github.com/anhkhoi121334/github-readme-stats">
    <img width="49%" src="https://github-readme-stats.vercel.app/api?username=anhkhoi121334&show_icons=true&theme=radical&hide_border=true&include_all_commits=true&count_private=true" />
  </a>
  <a href="https://github.com/anhkhoi121334/github-readme-stats">
    <img width="49%" src="https://github-readme-streak-stats.herokuapp.com/?user=anhkhoi121334&theme=radical&hide_border=true" />
  </a>
</div>

<div align="center">
  <a href="https://github.com/anhkhoi121334/github-readme-stats">
    <img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anhkhoi121334&layout=compact&theme=radical&hide_border=true&langs_count=8" />
  </a>
  <a href="https://github.com/anhkhoi121334">
    <img width="49%" src="https://github-profile-trophy.vercel.app/?username=anhkhoi121334&theme=radical&no-frame=true&no-bg=true&margin-w=10&row=2&column=4" />
  </a>
</div>

<br clear="both"/>

## 🌐 Let's Connect

<div align="center">
  <p>I'm always open to discussing new projects, creative ideas, or opportunities to be part of your vision.</p>
  
  <a href="mailto:khoi21007@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://www.facebook.com/Iamkhoicute.2004" target="_blank">
    <img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook" />
  </a>
  <a href="https://github.com/anhkhoi121334" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  
  <p>📫 How to reach me: <a href="mailto:khoi21007@gmail.com">khoi21007@gmail.com</a></p>
  
  <p>💼 Let's work together on your next project!</p>
</div>

---

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=anhkhoi121334&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />
  <p>Last Updated: November 18, 2025</p>
</div>
