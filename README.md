<!DOCTYPE html>
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 40px 20px;
    }

    .hero h1 {
      font-size: 64px;
      margin: 0;
      letter-spacing: 4px;
      text-transform: uppercase;
      text-shadow: 0 0 20px rgba(56,189,248,0.35);
    }

    .hero p {
      max-width: 700px;
      margin-top: 20px;
      font-size: 20px;
      color: #94a3b8;
    }

    .btn {
      margin-top: 30px;
      padding: 14px 28px;
      border: 1px solid #67e8f9;
      color: #67e8f9;
      border-radius: 12px;
      cursor: pointer;
      background: transparent;
    }

    footer {
      text-align: center;
      padding: 30px;
      color: #64748b;
    }
  </style>
</head>
<body>

  <div class="city"></div>
  <div class="car"></div>
  <div class="car"></div>
  <div class="rain"></div>

  <header>
    <div class="logo">NEON // SHAFIQ</div>
    <nav>
      <a href="#">Home</a>
      <a href="#">Journey</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Into The Night</h1>
    <p>Neon rain. Endless motion. Rebuilding yourself in the dark.</p>
    <button class="btn" onclick="toggleMusic()">Toggle Music</button>
  </section>

  <audio id="bgMusic" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/10/25/audio_946b6f1c82.mp3" type="audio/mpeg">
  </audio>

  <footer>
    © 2026 Shafiq // Cyberpunk Mode
  </footer>

  <script>
    const music = document.getElementById('bgMusic');

    function toggleMusic() {
      if (music.paused) {
        music.play();
      } else {
        music.pause();
      }
    }
  </script>

</body>
</html>
