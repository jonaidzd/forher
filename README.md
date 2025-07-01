# forher
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For You ♡</title>
  <link href="https://fonts.googleapis.com/css2?family=Caveat&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Caveat', cursive;
      background: linear-gradient(to bottom, #fce4ec, #e3f2fd);
      color: #333;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      text-align: center;
      overflow: hidden;
    }
    h1 {
      font-size: 3em;
    }
    p {
      font-size: 1.5em;
      margin: 10px 20px;
      max-width: 600px;
    }
    button {
      font-family: 'Caveat', cursive;
      font-size: 1.2em;
      padding: 10px 20px;
      background-color: #ffcccb;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      margin-top: 20px;
    }
    #complimentBox {
      margin-top: 20px;
      font-size: 1.3em;
      color: #444;
    }
    footer {
      position: absolute;
      bottom: 10px;
      font-size: 1em;
      color: #666;
    }
  </style>
</head>
<body>
  <h1>For the Sweetest Girl ♡</h1>
  <p>
    Hey beautiful,
    <br><br>
    I know things have been heavy lately. You’ve been pushing through stress and frustration like the strong, amazing soul you are. I made this little page just for you — a soft space to breathe, to smile, and to remember that I’m always here cheering for you.
    <br><br>
    You don’t need to have it all figured out. You don’t need to be perfect. You’re already enough — more than enough. You’re the most beautiful thing I’ve ever known, inside and out.
    <br><br>
    So whenever things get overwhelming, come here. I’ll be here in every pixel of this page. Loving you endlessly.
    <br><br>
    ♡ Always, your biggest fan.
  </p>

  <button onclick="showCompliment()">Click me for a smile :)</button>
  <div id="complimentBox"></div>

  <audio id="bgMusic" autoplay loop>
    <source src="https://hipstrumentals.com/wp-content/uploads/2024/04/Olivia-Rodrigo-happier-Instrumental-Prod.-By-Dan-Nigro.mp3" type="audio/mpeg">
  </audio>
  <button onclick="toggleMusic()">🎵 Toggle Music</button>

  <footer>
    Made with love, just for you ♡
  </footer>

  <script>
    const compliments = [
      "You light up every room you walk into.",
      "You are everything soft and strong wrapped in one.",
      "Even the moon envies your glow.",
      "You’re magic — don’t forget that.",
      "You make even the worst days better."
    ];

    function showCompliment() {
      const compliment = compliments[Math.floor(Math.random() * compliments.length)];
      document.getElementById("complimentBox").innerText = compliment;
    }

    function toggleMusic() {
      const music = document.getElementById("bgMusic");
      if (music.paused) {
        music.play();
      } else {
        music.pause();
      }
    }
  </script>
</body>
</html>
