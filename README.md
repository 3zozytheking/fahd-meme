# the gote 
index.html
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>💬 مقولات عزوزي الأسطورية 💬</title>
    <style>
        /* ضبط التنسيق بحيث يكون متجاوب */
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #ff4e50, #fc913a, #f9d423); 
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            padding: 10px;
        }

        h1 {
            font-size: 6vw; /* حجم متغير حسب الجهاز */
            text-shadow: 2px 2px 10px black;
        }

        button {
            padding: 12px 25px;
            font-size: 4vw; /* يجعل الزر أكبر على الجوال */
            font-weight: bold;
            background-color: #3b5998;
            color: white;
            border: none;
            cursor: pointer;
            margin-top: 20px;
            border-radius: 10px;
            transition: 0.3s;
        }

        button:hover {
            background-color: #1e2e5e;
            transform: scale(1.1);
        }

        .quote {
            font-size: 5vw; /* حجم النص يتناسب مع الجوال */
            margin-top: 20px;
            font-weight: bold;
            color: yellow;
            text-shadow: 2px 2px 5px black;
        }

        /* صندوق يحتوي على المقولات */
        .container {
            background: rgba(0, 0, 0, 0.6);
            padding: 15px;
            border-radius: 15px;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.5);
            max-width: 90%; /* يجعل التصميم مناسب للجوال */
        }

        /* استجابة خاصة للجوال */
        @media (max-width: 600px) {
            h1 {
                font-size: 8vw;
            }
            button {
                font-size: 5vw;
                padding: 10px 20px;
            }
            .quote {
                font-size: 6vw;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>🔥 مقولات عزوزي الأسطورية 🔥</h1>
        <p>📢 اضغط الزر لتحصل على حكمة من **عزوزي الفيلسوف**! 😂</p>

        <button onclick="showQuote()">🔮 اعطني حكمة 🔮</button>

        <p class="quote" id="quoteText"></p>
    </div>

    <script>
        function showQuote() {
            let quotes = [
                "😂 قنيصع أكثر واحد ينصح الناس، لكنه يحتاج نصيحة أول!",
                "🔥 اللي ما يعرف عزوزي، يعتبر نفسه ما عاش الحياة!",
                "🤣 يوم تفكر ترفع ضغط عزوزي، اعرف إنك تلعب بالنار!",
                "💀 البلاك بورد؟ نعمة إذا صار عن بعد، ونقمة إذا صرت مضطر تحضر!",
                "😂 المحاضرة بالفراش؟ رفاهية لا يفهمها إلا اللي يعشق النوم!",
                "🔥 إذا كنت بتواجه صعوبات، تذكر أنك مو قنيصع، فكل شيء سهل عليك!",
                "🤣 الدنيا يوم لك ويوم عليك، لكن قنيصع دايمًا عليه!",
                "💀 إذا قال عزوزي 'خلني أجرب'، فاعرف أن الابتكار في طريقه!",
                "😂 كل دقيقة مع عزوزي = 10 دقائق ضحك بدون توقف!",
                "🔥 سر النجاح؟ نام بدري، اشرب قهوة، وطقطق على قنيصع!"
            ];
            let randomIndex = Math.floor(Math.random() * quotes.length);
            document.getElementById("quoteText").innerText = quotes[randomIndex];
        }
    </script>

</body>
</html>
