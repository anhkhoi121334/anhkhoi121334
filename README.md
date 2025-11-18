<!-- GitHub Compatible Header with CSS Animation -->
<div align="center">
  
  <!-- Animated SVG Background -->
  <svg width="800" height="200" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" style="stop-color:#0f2027;stop-opacity:1" />
        <stop offset="50%" style="stop-color:#203a43;stop-opacity:1" />
        <stop offset="100%" style="stop-color:#2c5364;stop-opacity:1" />
      </linearGradient>
      
      <!-- Particle Animation -->
      <circle id="particle" r="2" fill="#4facfe" opacity="0.8">
        <animateMotion dur="20s" repeatCount="indefinite">
          <path d="M50,50 Q400,20 750,50 T750,150 Q400,180 50,150 T50,50"/>
        </animateMotion>
        <animate attributeName="opacity" values="0.3;1;0.3" dur="4s" repeatCount="indefinite"/>
      </circle>
    </defs>
    
    <!-- Background -->
    <rect width="100%" height="100%" fill="url(#bgGradient)" rx="10"/>
    
    <!-- Animated Particles -->
    <use href="#particle" transform="translate(0,0)">
      <animateTransform attributeName="transform" type="translate" 
        values="0,0; 50,30; 100,0; 50,-30; 0,0" dur="8s" repeatCount="indefinite"/>
    </use>
    <use href="#particle" fill="#00f2fe" transform="translate(100,50)">
      <animateTransform attributeName="transform" type="translate" 
        values="100,50; 150,20; 200,50; 150,80; 100,50" dur="10s" repeatCount="indefinite"/>
    </use>
    <use href="#particle" fill="#5ee7df" transform="translate(200,30)">
      <animateTransform attributeName="transform" type="translate" 
        values="200,30; 250,60; 300,30; 250,0; 200,30" dur="12s" repeatCount="indefinite"/>
    </use>
    <use href="#particle" fill="#667eea" transform="translate(300,70)">
      <animateTransform attributeName="transform" type="translate" 
        values="300,70; 350,40; 400,70; 350,100; 300,70" dur="9s" repeatCount="indefinite"/>
    </use>
    <use href="#particle" fill="#4facfe" transform="translate(400,40)">
      <animateTransform attributeName="transform" type="translate" 
        values="400,40; 450,70; 500,40; 450,10; 400,40" dur="11s" repeatCount="indefinite"/>
    </use>
    <use href="#particle" fill="#00f2fe" transform="translate(500,60)">
      <animateTransform attributeName="transform" type="translate" 
        values="500,60; 550,30; 600,60; 550,90; 500,60" dur="13s" repeatCount="indefinite"/>
    </use>
    <use href="#particle" fill="#5ee7df" transform="translate(600,25)">
      <animateTransform attributeName="transform" type="translate" 
        values="600,25; 650,55; 700,25; 650,-5; 600,25" dur="7s" repeatCount="indefinite"/>
    </use>
    <use href="#particle" fill="#667eea" transform="translate(700,55)">
      <animateTransform attributeName="transform" type="translate" 
        values="700,55; 750,25; 800,55; 750,85; 700,55" dur="14s" repeatCount="indefinite"/>
    </use>
    
    <!-- Text Content -->
    <text x="400" y="80" text-anchor="middle" fill="white" font-size="28" font-weight="bold" font-family="Arial">
      Hi there 👋, I'm Khôi
    </text>
    <text x="400" y="110" text-anchor="middle" fill="white" font-size="16" opacity="0.9" font-family="Arial">
      Frontend Developer (ReactJS)
    </text>
  </svg>

  <!-- Social Links -->
  <p>
    <a href="https://linkedin.com/in/anhkhoi121334">
      <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
    </a>
    <a href="mailto:khoi21007@gmail.com">
      <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
    </a>
    <a href="https://github.com/anhkhoi121334">
      <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
    </a>
  </p>

  <!-- Profile Views -->
  <p>
    <img src="https://komarev.com/ghpvc/?username=anhkhoi121334&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />
  </p>

</div>

<p align="center">
  Sinh viên mới tốt nghiệp, định hướng theo mảng Frontend Development.<br/>
  Mình tập trung vào xây dựng giao diện web hiện đại với ReactJS, responsive và dễ sử dụng.<br/>
  Luôn chủ động học hỏi, thực hành qua các dự án cá nhân để nâng cao kỹ năng.
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

Mini website thương mại điện tử bán giày, dùng để luyện tập ReactJS và quản lý state.

- **Tech Stack**: ReactJS, TailwindCSS, Zustand, REST API  
- **Features**:
  - Xem danh sách và chi tiết sản phẩm  
  - Thêm/xoá sản phẩm trong giỏ hàng  
  - Đăng nhập / đăng ký người dùng (luồng cơ bản)  
  - Giao diện responsive trên nhiều thiết bị  

---

### 💻 E-commerce Electronics Store
[![GitHub FE](https://img.shields.io/badge/Frontend_Repo-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anhkhoi121334/my-phim/tree/master/font-end)
[![GitHub BE](https://img.shields.io/badge/Backend_Repo-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anhkhoi121334/my-phim/tree/master/back-end)

Dự án web bán hàng điện tử, tách riêng Frontend và Backend để luyện tập mô hình fullstack.

- **Tech Stack**: ReactJS, TailwindCSS, Zustand, Node.js, Express, MongoDB  
- **Features**:
  - Hiển thị danh sách & chi tiết sản phẩm  
  - Giỏ hàng cơ bản  
  - Đăng nhập / đăng ký (cơ bản)  
  - Tạo và lưu đơn hàng phía backend  

<br>

## 📊 GitHub Stats

<div align="center">
  <a href="https://github.com/anhkhoi121334">
    <img width="49%" src="https://github-readme-stats.vercel.app/api?username=anhkhoi121334&show_icons=true&theme=radical&hide_border=true&include_all_commits=true&count_private=true" />
  </a>
  <a href="https://github.com/anhkhoi121334">
    <img width="49%" src="https://github-readme-streak-stats.herokuapp.com/?user=anhkhoi121334&theme=radical&hide_border=true" />
  </a>
</div>

<div align="center">
  <a href="https://github.com/anhkhoi121334">
    <img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anhkhoi121334&layout=compact&theme=radical&hide_border=true&langs_count=8" />
  </a>
  <a href="https://github.com/anhkhoi121334">
    <img width="49%" src="https://github-profile-trophy.vercel.app/?username=anhkhoi121334&theme=radical&no-frame=true&no-bg=true&margin-w=10&row=2&column=4" />
  </a>
</div>

<br clear="both"/>

## 🌐 Let's Connect

<div align="center">
  <p>Nếu anh/chị quan tâm đến các dự án của em hoặc cần hỗ trợ Frontend, em rất sẵn sàng trao đổi thêm ạ.</p>
  
  <a href="mailto:khoi21007@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://www.facebook.com/Iamkhoicute.2004" target="_blank">
    <img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook" />
  </a>
  <a href="https://github.com/anhkhoi121334" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</div>

---
