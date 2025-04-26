<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Birthday Ayang!</title>
  <style>
    body {
      background: linear-gradient(to right, #ffdde1, #ee9ca7);
      font-family: 'Comic Sans MS', cursive, sans-serif;
      text-align: center;
      padding: 50px;
      overflow: hidden;
    }

    .card {
      background-color: rgba(255, 255, 255, 0.2);
      padding: 30px;
      border-radius: 20px;
      display: inline-block;
      color: #fff;
      box-shadow: 0 0 15px rgba(0,0,0,0.3);
    }

    h1 {
      font-size: 3em;
      animation: shake 0.5s infinite;
    }

    p {
      font-size: 1.3em;
      margin-top: 10px;
    }

    @keyframes shake {
      0% { transform: translateX(0); }
      25% { transform: translateX(-5px); }
      50% { transform: translateX(5px); }
      75% { transform: translateX(-5px); }
      100% { transform: translateX(0); }
    }

    .confetti {
      position: absolute;
      width: 10px;
      height: 10px;
      background-color: #fff;
      animation: fall 4s linear infinite;
    }

    @keyframes fall {
      0% { transform: translateY(0) rotate(0deg); }
      100% { transform: translateY(100vh) rotate(360deg); }
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <div class="card">
    <h1>Happy Birthday Ayang!</h1>
    <p>Semoga panjang umur, sehat, pokoknya for all the best</p>
    <p>Dan semoga rencana pernikahan yg kita rencanakan bisa berjalan lancar dan terkabul.</p>
    <p>Love you always!</p>
  </div>

  <!-- Confetti Generator -->
  <script>
    for (let i = 0; i < 100; i++) {
      const confetti = document.createElement('div');
      confetti.classList.add('confetti');
      confetti.style.left = Math.random() * 100 + 'vw';
      confetti.style.animationDuration = (Math.random() * 3 + 2) + 's';
      confetti.style.backgroundColor = `hsl(${Math.random() * 360}, 100%, 70%)`;
      document.body.appendChild(confetti);
    }
  </script>
</body>
</html>
