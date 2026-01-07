<div align="center">

<svg width="800" height="200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="gradient1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#36BCF7;stop-opacity:1">
        <animate attributeName="stop-color" values="#36BCF7;#00f2fe;#36BCF7" dur="3s" repeatCount="indefinite"/>
      </stop>
      <stop offset="50%" style="stop-color:#00f2fe;stop-opacity:1">
        <animate attributeName="stop-color" values="#00f2fe;#36BCF7;#00f2fe" dur="3s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" style="stop-color:#36BCF7;stop-opacity:1">
        <animate attributeName="stop-color" values="#36BCF7;#00f2fe;#36BCF7" dur="3s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    
    <filter id="glow">
      <feGaussianBlur stdDeviation="4" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="shadow">
      <feDropShadow dx="0" dy="0" stdDeviation="8" flood-color="#36BCF7" flood-opacity="0.5"/>
    </filter>
  </defs>

  <!-- Arka plan -->
  <rect width="800" height="200" fill="#0a0e27"/>
  
  <!-- Animasyonlu partiküller -->
  <circle cx="100" cy="50" r="2" fill="#36BCF7" opacity="0.6">
    <animate attributeName="cy" from="200" to="-20" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.6;0.6;0" dur="8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="200" cy="120" r="2" fill="#00f2fe" opacity="0.6">
    <animate attributeName="cy" from="200" to="-20" dur="10s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.6;0.6;0" dur="10s" repeatCount="indefinite"/>
  </circle>
  <circle cx="350" cy="80" r="2" fill="#36BCF7" opacity="0.6">
    <animate attributeName="cy" from="200" to="-20" dur="9s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.6;0.6;0" dur="9s" repeatCount="indefinite"/>
  </circle>
  <circle cx="500" cy="140" r="2" fill="#00f2fe" opacity="0.6">
    <animate attributeName="cy" from="200" to="-20" dur="11s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.6;0.6;0" dur="11s" repeatCount="indefinite"/>
  </circle>
  <circle cx="650" cy="60" r="2" fill="#36BCF7" opacity="0.6">
    <animate attributeName="cy" from="200" to="-20" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.6;0.6;0" dur="7s" repeatCount="indefinite"/>
  </circle>

  <!-- Glow efekti -->
  <ellipse cx="400" cy="100" rx="300" ry="60" fill="url(#gradient1)" opacity="0.1" filter="url(#glow)">
    <animate attributeName="opacity" values="0.1;0.2;0.1" dur="2s" repeatCount="indefinite"/>
  </ellipse>

  <!-- Ana yazı -->
  <text x="400" y="120" font-family="'Arial Black', sans-serif" font-size="72" font-weight="800" text-anchor="middle" letter-spacing="4" filter="url(#shadow)">
    <tspan fill="url(#gradient1)">Ali Enes</tspan>
    <tspan fill="#ffffff" dx="15">ERSÖZLÜ</tspan>
  </text>

  <!-- Alt çizgi animasyonu -->
  <line x1="150" y1="145" x2="150" y2="145" stroke="url(#gradient1)" stroke-width="3" filter="url(#glow)">
    <animate attributeName="x2" from="150" to="650" dur="2s" fill="freeze"/>
  </line>
</svg>

<img 
  src="https://raw.githubusercontent.com/Aeerszl/aliee-library/main/images/github3d.gif"
  width="600"
  style="
    border-radius:20px;
    box-shadow:0 20px 40px rgba(0,0,0,.6);
    margin:20px 0;
  "
/>

<p>


  <span style="
    color:#E4405F;
    background:#0d1117;
    padding:8px 16px;
    border-radius:12px;
    border:1px solid #E4405F;
    font-weight:600;
    display:inline-block;
  ">
    🚀 Software Developer
  </span>
</p>

</div>

---

---

## 🌐 Connect with me:

<div align="center" style="margin: 30px 0;">
  
  <a href="linkedin.com/in/ali-enes-ersözlü-37a135256" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" style="margin: 10px;" />
  </a>
  
  <a href="mailto:aliee.developer@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" style="margin: 10px;" />
  </a>
  
  <a href="Aliee.dev" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" style="margin: 10px;" />
  </a>

</div>

---

## 🚀 Languages and Tools:

<div align="center">

<table>
  <tr>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=html" width="48" height="48" alt="HTML" />
      <br>HTML
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=css" width="48" height="48" alt="CSS" />
      <br>CSS
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=js" width="48" height="48" alt="JavaScript" />
      <br>JavaScript
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=ts" width="48" height="48" alt="TypeScript" />
      <br>TypeScript
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=react" width="48" height="48" alt="React" />
      <br>React
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=vue" width="48" height="48" alt="Vue.js" />
      <br>Vue.js
    </td>
  </tr>
  <tr>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=tailwind" width="48" height="48" alt="Tailwind" />
      <br>Tailwind
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=bootstrap" width="48" height="48" alt="Bootstrap" />
      <br>Bootstrap
    </td>
    <td align="center" width="96">
      <img src="https://raw.githubusercontent.com/saadeghi/daisyui-images/master/images/daisyui-logo/favicon-192.png" width="48" height="48" alt="DaisyUI" />
      <br>DaisyUI
    </td>
    <td align="center" width="96">
      <img src="https://avatars.githubusercontent.com/u/139895814?s=200&v=4" width="48" height="48" alt="Shadcn" />
      <br>Shadcn UI
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=jquery" width="48" height="48" alt="jQuery" />
      <br>jQuery
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=php" width="48" height="48" alt="PHP" />
      <br>PHP
    </td>
  </tr>
  <tr>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=nodejs" width="48" height="48" alt="Node.js" />
      <br>Node.js
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=express" width="48" height="48" alt="Express" />
      <br>Express
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=wordpress" width="48" height="48" alt="WordPress" />
      <br>WordPress
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=postgresql" width="48" height="48" alt="PostgreSQL" />
      <br>PostgreSQL
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=flutter" width="48" height="48" alt="Flutter" />
      <br>Flutter
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=react" width="48" height="48" alt="React Native" />
      <br>React Native
    </td>
  </tr>
  <tr>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=git" width="48" height="48" alt="Git" />
      <br>Git
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=github" width="48" height="48" alt="GitHub" />
      <br>GitHub
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=vscode" width="48" height="48" alt="VS Code" />
      <br>VS Code
    </td>
    <td align="center" width="96">
      <img src="https://skillicons.dev/icons?i=postman" width="48" height="48" alt="Postman" />
      <br>Postman
    </td>
  </tr>
</table>

</div>

---

<div align="center">
  <i>⭐️ From <a href="https://github.com/YOUR_GITHUB_USERNAME">Ali Enes ERSÖZLÜ</a></i>
</div>
