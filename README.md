# the gote 
index.html
<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>رسالة اعتذار من عزوزي إلى دُنا</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #6a11cb, #2575fc); /* خلفية رايقة */
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      padding: 10px;
      overflow: hidden;
      position: relative;
    }

    h1 {
      font-size: 3em;
      text-shadow: 2px 2px 10px black;
      animation: fadeIn 3s ease-out;
    }

    .message-box {
      font-size: 1.5em;
      width: 80%;
      text-align: center;
      margin-top: 20px;
      opacity: 0;
      animation: fadeMessage 3s ease-out forwards;
    }

    button {
      padding: 12px 30px;
      font-size: 18px;
      font-weight: bold;
      background-color: #ff6347;
      border-radius: 5px;
      border: none;
      color: white;
      margin-top: 20px;
      cursor: pointer;
      animation: bounce 2s infinite;
    }

    button:hover {
      background-color: #ff4500;
    }

    .hearts {
      position: absolute;
      top: 10%;
      left: 50%;
      transform: translateX(-50%);
      animation: floatingHearts 3s ease-in-out infinite;
    }

    .heart {
      font-size: 3em;
      color: #ff69b4;
      animation: heartBounce 1.5s infinite;
      margin: 0 5px;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes fadeMessage {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes bounce {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.1); }
    }

    @keyframes floatingHearts {
      0% { top: 10%; opacity: 0.8; }
      50% { top: 20%; opacity: 1; }
      100% { top: 10%; opacity: 0.8; }
    }

    @keyframes heartBounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
  </audio>

  <div class="hearts">
    <span class="heart">💖</span>
    <span class="heart">💖</span>
    <span class="heart">💖</span>
    <span class="heart">💖</span>
  </div>

  <div>
    <h1>رسالة اعتذار من عزوزي إلى دُنا</h1>
    <div class="message-box">
      <p>عزيزتي **دُنا**،<br><br>
      أنا أعلم أن الأيام الماضية كانت مليئة بالتصرفات التي لم تعكس شخصيتي الحقيقية،<br><br>
      ولكني اليوم أدرك تمامًا أن **الخطأ** كان في تصرفاتي تجاهك.<br><br>
      **دُنا**، أنتِ شخص عزيز جدًا على قلبي، وأنا **أعتذر** عن أي تصرف أو كلمة غير لائقة صدرت مني في تلك الفترة.<br><br>
      لا يمكنني العيش مع فكرة أنني **أقللت** من قيمتك أو أسأت إليك.<br><br>
      أتمنى أن تقبلي اعتذاري، وأعدك أنني سأبذل كل جهدي لكي لا أكرر **هذا الخطأ**.<br><br>
      مع خالص اعتذاري،<br><br>
      **عزوزي**</p>
    </div>
    <button onclick="alert('تم إرسال الرسالة بنجاح!')">إرسال الرسالة</button>
  </div>
  
</body>
</html>
