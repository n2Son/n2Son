- 👋 Hi, I’m @n2Son
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
n2Son/n2Son is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
  <style>
    body {
      margin: 0;
      padding: 0;
      overflow: hidden;
    }
    
    .snowflakes {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 9999;
    }

    .flake {
      position: absolute;
      background: white;
      width: 10px;
      height: 10px;
      border-radius: 50%;
      opacity: 0.7;
      animation: falling linear infinite;
    }

    @keyframes falling {
      0% {
        transform: translateY(-100%);
      }
      
      100% {
        transform: translateY(100vh);
      }
    }

    .text-effect {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 40px;
      font-weight: bold;
      color: white;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
      z-index: 9999;
    }
  </style>
</head>
<body>
  <div class="snowflakes"></div>
  <div class="text-effect">Nguyen Ngoc Son</div>

  <script>
    function createSnow() {
      const flakes = document.querySelector(".snowflakes");

      for (let i = 0; i < 50; i++) {
        const flake = document.createElement("div");
        flake.className = "flake";
        flakes.appendChild(flake);
      }
    }

    createSnow();
  </script>
