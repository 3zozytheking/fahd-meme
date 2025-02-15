# know 
index.html
 <!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تحدي من يعرف عزوزي؟ 🔥</title>
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
        .question {
            font-size: 22px;
            margin-top: 20px;
            color: #333;
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
        .result {
            font-size: 24px;
            margin-top: 20px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <h1>🔥 تحدي: من يعرف عزوزي أكثر؟ 🔥</h1>
    <p>جاوب على الأسئلة واكتشف إذا كنت من **المقربين** أو مجرد واحد مثل قنيصع! 😂</p>

    <div id="quiz">
        <div class="question" id="questionText"></div>
        <button onclick="checkAnswer(0)">1</button>
        <button onclick="checkAnswer(1)">2</button>
        <button onclick="checkAnswer(2)">3</button>
        <button onclick="checkAnswer(3)">4</button>
    </div>

    <p class="result" id="resultText"></p>

    <script>
        let questions = [
            { 
                question: "ما هو تخصص عزوزي في الجامعة؟",
                options: ["هندسة", "طب", "تقنية معلومات (IT)", "قانون"],
                correct: 2
            },
            { 
                question: "ما هو اسم فهد الحقيقي؟ 😂",
                options: ["قنيصع", "فهد", "أبو ناصر", "سلطان"],
                correct: 1
            },
            { 
                question: "ما هو العطر المفضل لعزوزي؟",
                options: ["ديور سوفاج", "بلو دي شانيل", "Allure Homme Sport", "لا يستخدم عطور"],
                correct: 2
            },
            { 
                question: "ما هو المسلسل الكوميدي المفضل عند عزوزي؟",
                options: ["Friends", "The Office", "How I Met Your Mother", "Brooklyn Nine-Nine"],
                correct: 2
            },
            { 
                question: "ماذا يفضل عزوزي في الفتيات؟",
                options: ["الشعر الطويل الأشقر", "البشرة السمراء والعينين العسلية", "العيون الخضراء", "القصيرات فقط"],
                correct: 1
            },
            { 
                question: "ما هو اسم ابن عزوزي المستقبلي؟",
                options: ["فارس", "محمد", "عبدالله", "ماجد"],
                correct: 1
            },
            { 
                question: "ماذا يكره عزوزي؟",
                options: ["رائحة الثوم والزيت", "الطقس البارد", "القطط", "الأكل الحار"],
                correct: 0
            },
            { 
                question: "من هو العدو الأبدي لعزوزي؟",
                options: ["قنيصع", "أحد أساتذته", "زميل عمله", "فريقه المفضل إذا خسر"],
                correct: 0
            }
        ];

        let currentQuestion = 0;
        let score = 0;

        function loadQuestion() {
            if (currentQuestion < questions.length) {
                document.getElementById("questionText").innerText = questions[currentQuestion].question;
                let buttons = document.getElementsByTagName("button");
                for (let i = 0; i < 4; i++) {
                    buttons[i].innerText = questions[currentQuestion].options[i];
                }
            } else {
                showResult();
            }
        }

        function checkAnswer(answer) {
            if (answer === questions[currentQuestion].correct) {
                score++;
            }
            currentQuestion++;
            loadQuestion();
        }

        function showResult() {
            let resultText = "";
            if (score === questions.length) {
                resultText = "🔥🔥 أسطوري! أنت تعرف عزوزي أكثر مما يعرف نفسه! 🔥🔥";
            } else if (score >= questions.length / 2) {
                resultText = "😂 جيد! لكن تحتاج تعرف عزوزي أكثر.";
            } else {
                resultText = "💀 قنيصع أنت؟ واضح إنك ما تعرف شيء!";
            }
            document.getElementById("quiz").style.display = "none";
            document.getElementById("resultText").innerText = resultText;
        }

        loadQuestion();
    </script>

</body>
</html>
       
