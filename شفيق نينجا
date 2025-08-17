<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <title>لاعب كرة القدم المتقدم</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Cairo', sans-serif;
      background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/4/4d/Soccer_pitch_blank.svg/1024px-Soccer_pitch_blank.svg.png') no-repeat center center fixed;
      background-size: cover;
      margin: 0;
      padding: 0;
    }

    .header {
      background: rgba(80,125,188,0.9);
      color: #fff;
      padding: 2rem;
      text-align: center;
      font-size: 24px;
      font-weight: bold;
      box-shadow: 0px 4px 10px rgba(0,0,0,0.3);
    }

    .main-content {
      max-width: 900px;
      margin: 30px auto;
      padding: 20px;
      background: rgba(255,255,255,0.9);
      border-radius: 15px;
      box-shadow: 0px 4px 15px rgba(0,0,0,0.2);
      text-align: center;
    }

    .story-article h2 {
      color: #507DBC;
      font-size: 28px;
      margin-bottom: 15px;
    }

    .story-article p {
      font-size: 16px;
      line-height: 1.6;
      margin-bottom: 15px;
      animation: fadeIn 2s ease-in;
    }

    .intro {
      font-weight: bold;
      color: #444;
    }

    #counter {
      font-size: 50px;
      font-weight: bold;
      color: #507DBC;
      margin: 20px 0;
    }

    .player-container {
      position: relative;
      width: 200px;
      height: 200px;
      margin: 20px auto;
    }

    .player {
      width: 150px;
      position: absolute;
      bottom: 0;
      left: 25px;
      animation: playerMove 1s infinite alternate ease-in-out;
      z-index: 1;
    }

    .ball {
      width: 50px;
      position: absolute;
      top: 70px;
      left: 120px;
      transform-origin: center center;
      animation: ballCircle 1s infinite linear;
      z-index: 2;
    }

    .ad-container {
      background: #ffffff;
      border: 1px dashed #ccc;
      padding: 20px;
      margin: 30px;
      text-align: center;
    }

    .ad-container p {
      color: #507DBC;
      font-style: italic;
    }

    .footer {
      text-align: center;
      background: rgba(255,255,255,0.9);
      color: #333333;
      margin-top: 60px;
      padding: 20px;
      font-size: 14px;
      border-radius: 10px;
      box-shadow: 0px 4px 10px rgba(0,0,0,0.2);
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes playerMove {
      0% { transform: rotate(0deg) translateY(0); }
      50% { transform: rotate(-5deg) translateY(-10px); }
      100% { transform: rotate(0deg) translateY(0); }
    }

    @keyframes ballCircle {
      0%   { transform: rotate(0deg) translateX(30px) rotate(0deg); }
      25%  { transform: rotate(90deg) translateX(30px) rotate(-90deg); }
      50%  { transform: rotate(180deg) translateX(30px) rotate(-180deg); }
      75%  { transform: rotate(270deg) translateX(30px) rotate(-270deg); }
      100% { transform: rotate(360deg) translateX(30px) rotate(-360deg); }
    }
  </style>
</head>
<body>

  <div class="header">⚽ لاعب كرة القدم المتقدم</div>

  <div class="main-content">
    <div class="story-article">
      <h2>اللاعب النشيط</h2>
      <p class="intro">اللاعب يتحرك ويكمل الكرة حول قدميه!</p>

      <div class="player-container">
        <img src="https://upload.wikimedia.org/wikipedia/commons/8/8f/Soccer_player_icon.svg" alt="لاعب" class="player">
        <img src="https://upload.wikimedia.org/wikipedia/commons/3/36/Soccerball.svg" alt="كرة القدم" class="ball" id="soccerBall">
      </div>

      <p>العد التنازلي لمتابعة الحركة:</p>
      <p id="counter">10</p>
    </div>

    <div class="ad-container">
      <p>📢 جرب هذه الحركات بنفسك وتحدى أصدقاءك!</p>
    </div>
  </div>

  <div class="footer" id="finalMessage">© 2025 بدر - كل الحقوق محفوظة</div>

  <audio id="kickSound" src="https://www.soundjay.com/button/beep-07.wav"></audio>

  <script>
    // العد التنازلي
    let count = 10;
    let counter = document.getElementById('counter');
    let finalMsg = document.getElementById('finalMessage');
    let ball = document.getElementById('soccerBall');
    let kick = document.getElementById('kickSound');

    let interval = setInterval(() => {
      counter.innerText = count;
      kick.play(); // تشغيل صوت الركلة
      count--;
      if(count < 0) {
        clearInterval(interval);
        finalMsg.innerText = "🎉 انتهى العد! جربها أنت أيضًا! ⚽";
      }
    }, 1000);
  </script>

</body>
</html>
