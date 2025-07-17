# I love you tiny 
<!DOCTYPE html>
<html lang="en">
<head>
  …
  <style>
    /* Existing styles… */
    #whale {
      width: 200px;
      position: absolute;
      bottom: 20px;
      right: 20px;
      animation: swim 4s ease-in-out infinite alternate;
    }
    @keyframes swim {
      from { transform: translateX(0) rotate(0); }
      to { transform: translateX(-20px) rotate(-2deg); }
    }
  </style>
</head>
<body>
  <div id="container">
    …
    <button onclick="startCelebration()">✨ Celebrate Now!</button>
  </div>

  <!-- 🎵 and confetti script -->

  <!-- Whale image -->
  <img id="whale"
       src="https://images.freepik.com/free-vector/cute-whale-birthday-party-childish-design_33058868.jpg"
       alt="Cute birthday whale" />

  <!-- Scripts… -->
</body>
</html>
