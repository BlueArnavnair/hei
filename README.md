# hei
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Happy Birthday!</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: url('https://source.unsplash.com/1600x900/?birthday,balloons') no-repeat center/cover;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      text-align: center;
      color: #fff;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
    h1 {
      font-size: 4em;
      text-shadow: 2px 2px 4px #000;
      animation: pulse 1s infinite;
    }
    p {
      font-size: 1.5em;
      animation: fade-in 3s forwards;
      opacity: 0;
    }
    @keyframes pulse {
      0%, 100% {transform: scale(1);}
      50% {transform: scale(1.05);}
    }
    @keyframes fade-in {
      to {opacity: 1;}
    }
    button {
      margin-top: 20px;
      padding: 15px 30px;
      font-size: 1em;
      border: none;
      border-radius: 8px;
      background: #ff4081;
      color: #fff;
      cursor: pointer;
      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    }
    button:hover {
      background: #e73370;
    }
  </style>
</head>
<body>
  <h1>🎉 Happy Birthday, [Friend's Name]! 🎂</h1>
  <p id="wish">Wishing you a day full of joy, love & amazing surprises!</p>
  <button onclick="playTunes()">🎵 Play Celebration Music!</button>

  <audio id="bgMusic" src="https://your-audio-source.mp3" loop></audio>

  <script>
    function playTunes() {
      const audio = document.getElementById('bgMusic');
      audio.play();
    }
    window.addEventListener('DOMContentLoaded', () => {
      document.getElementById('wish').style.opacity = 1;
    });
  </script>
</body>
</html>
