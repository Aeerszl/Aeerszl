<h1 align="center">Hi 👋, I'm Ali Enes ERSÖZLÜ</h1>
<div align="center">
<h3>I am Computer Engineer Student (web developer)</h3>
  
<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ali Enes 3D Cube</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100vw;
      height: 100vh;
      perspective: 6000px;
      background: #000;
      overflow: hidden;
      margin: 0;
    }

    #wrap {
      zoom: 0.9;
      width: 350px;
      height: 350px;
      position: relative;
      transform-style: preserve-3d;
      animation: updown 5s ease-in-out infinite alternate;
      transform-origin: 50% 100%;
    }

    #wrap:before {
      content: '';
      position: absolute;
      width: 400%;
      height: 400%;
      left: -150%;
      top: -150%;
      background: radial-gradient(ellipse at center, #000 0%, transparent 90%);
      backface-visibility: hidden;
      animation: fade 5s ease-in-out infinite alternate;
      border-radius: 100%;
    }

    @keyframes fade {
      0% { transform: scale(0); opacity: 0; }
      75% { transform: scale(0.25); opacity: 1; }
      97.5% { transform: scale(1); }
      100% { transform: scale(1); }
    }

    @keyframes updown {
      0%, 10% {
        transform: scale(0.75) translateY(-15%) rotateX(60deg) scaleY(1.75);
        transform-origin: 50% 75%;
      }
      90%, 100% {
        transform: scale(0.75) rotateX(0deg) translateY(12.5%);
        transform-origin: 50% 0%;
      }
    }

    .cube {
      position: absolute;
      width: 100%;
      height: 33.3333%;
      left: 0;
      transform-style: preserve-3d;
      transform: rotateX(0deg) rotateY(315deg);
      animation: spinback 5s ease-in-out infinite;
    }

    .cube:nth-of-type(1) { top: 0%; }
    .cube:nth-of-type(2) { top: 30%; animation-direction: reverse; }
    .cube:nth-of-type(3) { top: 60%; }

    .cube:nth-of-type(even) * { animation-direction: reverse; }
    .cube:nth-of-type(even) *:before { animation-direction: reverse !important; }

    @keyframes spinback {
      10% { transform: rotateX(0deg) rotateY(315deg); }
      90%, 100% { transform: rotateX(0deg) rotateY(-45deg); }
    }

    @keyframes spinback2 {
      10% { transform: rotateX(0deg) rotateY(-315deg); }
      90%, 100% { transform: rotateX(0deg) rotateY(45deg); }
    }

    @keyframes spinback3 {
      10% { transform: rotateX(0deg) rotateY(-315deg); }
      90%, 100% { transform: rotateX(0deg) rotateY(45deg); }
    }

    .cube div {
      position: absolute;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      transform-style: preserve-3d;
    }

    .cube div * {
      transform-style: preserve-3d;
    }

    .cube h1 {
      width: calc(100% - 10px);
      left: 5px;
      position: relative;
      margin: 0;
      font-size: 50px;
      font-weight: 900;
      font-family: Futura, Arial, sans-serif;
      height: 100%;
      display: flex;
      justify-content: center;
    }

    .word {
      position: relative;
      width: 100%;
      display: flex;
    }

    .char {
      display: flex;
      justify-content: center;
      align-items: center;
      flex: 1;
      height: 100%;
      color: transparent;
    }

    .char:before {
      content: attr(data-char);
      color: #fff;
      font-weight: 900;
      -webkit-text-stroke: 5px #000;
      position: absolute;
      transform: rotateX(0deg) rotateY(-315deg);
      animation: spinback2 5s ease-in-out infinite;
      text-shadow: 0 0 40px #000;
    }

    .front {
      transform: translateZ(175px);
    }

    .front .char:nth-of-type(-n + 3):before {
      color: #000;
      -webkit-text-stroke: 3px #fff;
    }

    .back {
      transform: translateZ(-175px) rotateY(0deg) rotateX(0deg);
    }

    .back .char {
      transform: rotateY(360deg);
    }

    .back .char:nth-of-type(n + 4):before {
      color: #000;
      -webkit-text-stroke: 3px #fff;
    }

    .back .char:before {
      animation: spinback3 5s ease-in-out infinite;
    }

    .left {
      transform-origin: left;
      left: 100%;
      transform: translateZ(175px) rotateY(90deg);
    }

    .left .char {
      transform: rotateY(-90deg);
    }

    .right {
      transform-origin: right;
      left: -100%;
      transform: translateZ(175px) rotateY(-90deg);
    }

    .right .char {
      transform: rotateY(90deg);
    }
  </style>
</head>
<body>
  <div id="wrap">
    <div class="cube">
      <div class="front">
        <h1>
          <div class="word">
            <span class="char" data-char="A">A</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="I">I</span>
            <span class="char" data-char=" "> </span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="N">N</span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="S">S</span>
          </div>
        </h1>
      </div>
      <div class="left">
        <h1>
          <div class="word">
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="R">R</span>
            <span class="char" data-char="S">S</span>
            <span class="char" data-char="Ö">Ö</span>
            <span class="char" data-char="Z">Z</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="Ü">Ü</span>
          </div>
        </h1>
      </div>
      <div class="right">
        <h1>
          <div class="word">
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="R">R</span>
            <span class="char" data-char="S">S</span>
            <span class="char" data-char="Ö">Ö</span>
            <span class="char" data-char="Z">Z</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="Ü">Ü</span>
          </div>
        </h1>
      </div>
      <div class="back">
        <h1>
          <div class="word">
            <span class="char" data-char="A">A</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="I">I</span>
            <span class="char" data-char=" "> </span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="N">N</span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="S">S</span>
          </div>
        </h1>
      </div>
    </div>

    <div class="cube">
      <div class="front">
        <h1>
          <div class="word">
            <span class="char" data-char="A">A</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="I">I</span>
            <span class="char" data-char=" "> </span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="N">N</span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="S">S</span>
          </div>
        </h1>
      </div>
      <div class="left">
        <h1>
          <div class="word">
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="R">R</span>
            <span class="char" data-char="S">S</span>
            <span class="char" data-char="Ö">Ö</span>
            <span class="char" data-char="Z">Z</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="Ü">Ü</span>
          </div>
        </h1>
      </div>
      <div class="right">
        <h1>
          <div class="word">
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="R">R</span>
            <span class="char" data-char="S">S</span>
            <span class="char" data-char="Ö">Ö</span>
            <span class="char" data-char="Z">Z</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="Ü">Ü</span>
          </div>
        </h1>
      </div>
      <div class="back">
        <h1>
          <div class="word">
            <span class="char" data-char="A">A</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="I">I</span>
            <span class="char" data-char=" "> </span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="N">N</span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="S">S</span>
          </div>
        </h1>
      </div>
    </div>

    <div class="cube">
      <div class="front">
        <h1>
          <div class="word">
            <span class="char" data-char="A">A</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="I">I</span>
            <span class="char" data-char=" "> </span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="N">N</span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="S">S</span>
          </div>
        </h1>
      </div>
      <div class="left">
        <h1>
          <div class="word">
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="R">R</span>
            <span class="char" data-char="S">S</span>
            <span class="char" data-char="Ö">Ö</span>
            <span class="char" data-char="Z">Z</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="Ü">Ü</span>
          </div>
        </h1>
      </div>
      <div class="right">
        <h1>
          <div class="word">
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="R">R</span>
            <span class="char" data-char="S">S</span>
            <span class="char" data-char="Ö">Ö</span>
            <span class="char" data-char="Z">Z</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="Ü">Ü</span>
          </div>
        </h1>
      </div>
      <div class="back">
        <h1>
          <div class="word">
            <span class="char" data-char="A">A</span>
            <span class="char" data-char="L">L</span>
            <span class="char" data-char="I">I</span>
            <span class="char" data-char=" "> </span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="N">N</span>
            <span class="char" data-char="E">E</span>
            <span class="char" data-char="S">S</span>
          </div>
        </h1>
      </div>
    </div>
  </div>
</body>
</html>

</div>

---

## 🌐 Connect with me:

<div align="center" style="margin: 30px 0;">
  
  <a href="YOUR_LINKEDIN_URL" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" style="margin: 10px;" />
  </a>
  
  <a href="mailto:YOUR_EMAIL@example.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" style="margin: 10px;" />
  </a>
  
  <a href="YOUR_INSTAGRAM_URL" target="_blank">
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
