
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Forever Yours – Rukaya & Muzamil friendship forever</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins&display=swap" rel="stylesheet" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(to right, #ffdde1, #ee9ca7);
      color: #333;
      overflow-x: hidden;
      scroll-behavior: smooth;
      position: relative;
    }

    header {
      text-align: center;
      padding: 3rem 1rem 4rem;
      background-color: rgba(255, 255, 255, 0.2);
      backdrop-filter: blur(5px);
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3.5rem;
      color: #e60073;
      margin-bottom: 1rem;
    }

    p.quote {
      font-size: 1.2rem;
      font-style: italic;
    }

    section {
      padding: 3rem 1rem;
      max-width: 800px;
      margin: auto;
    }

    .timeline {
      border-left: 3px solid #e60073;
      padding-left: 1rem;
      position: relative;
    }

    .timeline::before {
      content: '';
      position: absolute;
      left: -9px;
      top: 0;
      width: 15px;
      height: 15px;
      background: #e60073;
      border-radius: 50%;
    }

    .timeline p {
      margin: 1rem 0;
    }

    .surprise {
      text-align: center;
      margin-top: 2rem;
    }

    .btn {
      padding: 1rem 2rem;
      background-color: #e60073;
      color: white;
      border: none;
      border-radius: 25px;
      font-size: 1rem;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .btn:hover {
      background-color: #c4005a;
    }

    footer {
      text-align: center;
      padding: 2rem;
      font-size: 0.9rem;
      color: #666;
    }
  #popup {
  display: none;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: white;
  padding: 2.5rem 3rem; /* Thoda aur padding for space */
  border-radius: 20px;
  box-shadow: 0px 0px 30px rgba(0, 0, 0, 0.3);
  z-index: 100;
  text-align: center;
  animation: fadeIn 0.5s ease;
  max-width: 95%; /* Pehle 90% tha, ab thoda bada */
  max-height: 80vh; /* Height control, scroll ho jayega agar text bada hua */
  overflow-y: auto; /* Agar height exceed kare to scroll ayega */
  word-wrap: break-word; /* Text wrap karne ke liye */
}

    #popup p {
      font-size: 1.3rem;
      color: #e60073;
      margin-top: 1rem;
    }

    #overlay {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.4);
      z-index: 99;
    }

    #popup img {
  max-width: 180px; /* Pehle 250px tha */
  width: 85%; /* Pehle 90% tha */
  border-radius: 20px;
  box-shadow: 0 0 30px rgba(255, 0, 119, 0.6);
  animation: pulse 2s infinite;
}
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translate(-50%, -60%);
      }
      to {
        opacity: 1;
        transform: translate(-50%, -50%);
      }
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.05); }
      100% { transform: scale(1); }
    }

    audio {
      display: none;
    }

    .heart-particles {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      overflow: hidden;
      z-index: 1;
      pointer-events: none;
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: url('https://i.imgur.com/kN1B1Gf.png') no-repeat center;
      background-size: cover;
      animation: float 8s infinite ease-in;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) scale(0.3);
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-10vh) scale(1);
        opacity: 0;
      }
    }

    #typing {
      font-weight: bold;
      font-size: 1.2rem;
      color: #e60073;
      white-space: nowrap;
      overflow: hidden;
      border-right: 2px solid #e60073;
      animation: typing 4s steps(40, end), blink 0.75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink {
      50% { border-color: transparent; }
    }
  </style>
</head>
<body>

  <div class="heart-particles" id="hearts-container"></div>

  <header>
    <h1>Forever Yours</h1><br>
    <h1>love you so much my dear bestie</h1>
    
    <p class="quote">"From a conference call to forever – our journey is written in the stars."</p>
  </header>

  <section>
    <h2>Our Story</h2>
    <div class="timeline">
      <p>📞 First call during Rukaya's breakup</p>
      <p>🤝 Friendship that became special</p>
      <p>💖 Love bloomed – 1 year 3 months strong</p>
      <p>🫶 Still going strong, forever to go...</p>
      
    </div>

    <div class="surprise">
      <button class="btn" onclick="showPopup()">Click for a Surprise 💌</button>
    </div>
  </section>

  <div id="overlay" onclick="hidePopup()"></div>
  <div id="popup">
    <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1744658409/Picsart_25-04-14_00-56-51-907_ztwdk2.jpg" alt="Rukaya & Muzamil" />
    <p id="typing">Rukaya, you are the reason behind Muzamil's smile 💫</p>
  </div>

  <footer>
    Made with 💕 by Muzamil | For Rukaya Only
  </footer>

  <audio id="romanticAudio" loop>
    <source src="https://media.vocaroo.com/mp3/1gTT0pHu0Nr7" type="audio/mpeg" />
    Your browser does not support the audio element.
  </audio>

  <script>
    const popup = document.getElementById('popup');
    const overlay = document.getElementById('overlay');
    const audio = document.getElementById('romanticAudio');

    function showPopup() {
      popup.style.display = 'block';
      overlay.style.display = 'block';
      audio.play();
      createHearts();
    }

    function hidePopup() {
      popup.style.display = 'none';
      overlay.style.display = 'none';
      audio.pause();
      audio.currentTime = 0;
    }

    function createHearts() {
      const container = document.getElementById("hearts-container");
      container.innerHTML = "";
      for (let i = 0; i < 30; i++) {
        const heart = document.createElement("div");
        heart.className = "heart";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.animationDuration = (5 + Math.random() * 5) + "s";
        container.appendChild(heart);
      }
    }
  </script>

</body>
</html>
