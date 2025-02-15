# the gote 
index.html
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>💬 مقولات عزوزي الأسطورية 💬</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            padding: 20px;
        }
        h1 {
            color: red;
            font-size: 40px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            background-color: #ff5733;
            color: white;
            border: none;
            cursor: pointer;
            margin-top: 20px;
            border-radius: 5px;
        }
        button:hover {
            background-color: #c70039;
        }
        .quote {
            font-size: 24px;
            margin-top: 20px;
            color: blue;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <h1>🔥 مقولات عزوزي الأسطورية 🔥</h1>
    <p>اضغط الزر لتحصل على حكمة من **عزوزي الفيلسوف**! 😂</p>

    <button onclick="showQuote()">🔮 اعطني حكمة 🔮</button>

    <p class="quote" id="quoteText"></p>

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
