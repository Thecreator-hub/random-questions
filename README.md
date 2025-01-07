<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fun Question Generator</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #74ebd5, #9face6);
      color: #fff;
      text-align: center;
      padding: 0 20px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }
    p {
      font-size: 1.2rem;
      margin-bottom: 30px;
    }
    button {
      padding: 15px 30px;
      font-size: 1rem;
      font-weight: bold;
      color: #fff;
      background: #ff7eb3;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button:hover {
      background: #ff528c;
    }
    .question-box {
      margin-top: 20px;
      padding: 20px;
      border: 2px solid #fff;
      border-radius: 10px;
      background: rgba(255, 255, 255, 0.2);
      font-size: 1.5rem;
      font-weight: bold;
      max-width: 600px;
      word-wrap: break-word;
    }
  </style>
</head>
<body>
  <h1>Fun Question Generator</h1>
  <p>Click the button below to get a random question for friends or loved ones!</p>
  <button onclick="generateQuestion()">Generate Question</button>
  <div class="question-box" id="questionDisplay">Your question will appear here.</div>

  <script>
    const questions = [
      "What’s your favorite childhood memory?",
      "If you could meet any celebrity, who would it be?",
      "What’s one thing you’d like to do before you die?",
      "Who inspires you the most in your life?",
      "What’s the most adventurous thing you’ve ever done?",
      "If you could live anywhere in the world, where would it be?",
      "What’s your favorite movie or TV series?",
      "If you won the lottery, what’s the first thing you’d buy?",
      "What’s your biggest fear?",
      "Who knows you best in the world?",
      "What’s the most embarrassing thing that’s ever happened to you?",
      "If you could have a superpower, what would it be?",
      "What’s the best trip you’ve ever been on?",
      "What’s your favorite food that you can’t live without?",
      "If you could change one thing about yourself, what would it be?",
      "What’s your biggest regret in life?",
      "What’s the funniest memory we share?",
      "If you could relive one day in your life, what day would it be?",
      "What’s your go-to comfort activity?",
      "Who was your first crush?",
      "What’s one thing you’ve never told anyone?",
      "If you could master any skill instantly, what would it be?",
      "What’s your dream job?",
      "What’s one thing that always makes you happy?",
      "If you could live in any time period, when would it be?",
      "What’s your guilty pleasure?",
      "If you could swap lives with someone for a day, who would it be?",
      "What’s the kindest thing someone has done for you?",
      "What’s a goal you’re working toward right now?",
      "What’s one thing you’d bring to a deserted island?"
      
    ];

    function generateQuestion() {
      const randomIndex = Math.floor(Math.random() * questions.length);
      const questionDisplay = document.getElementById("questionDisplay");
      questionDisplay.textContent = questions[randomIndex];
    }
  </script>
</body>
</html>
