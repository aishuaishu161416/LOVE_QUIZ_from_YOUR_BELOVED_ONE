<!DOCTYPE html>
<html>
<head>
  <title>Love Unlock Quiz</title>
  <style>
    body {
      background-color: #111;
      color: #fff;
      font-family: Arial, sans-serif;
      text-align: center;
      overflow: hidden;
    }
    .question {
      display: none;
      margin-top: 50px;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      background: #222;
      color: #fff;
      border: 2px solid pink;
      border-radius: 8px;
      transition: all 0.3s ease;
    }
    button:hover {
      background: pink;
      color: #111;
      box-shadow: 0 0 15px pink;
    }
    .success {
      color: pink;
      font-size: 22px;
      margin-top: 30px;
    }

    /* Glowing heart animation */
    .heart {
      color: hotpink;
      font-size: 40px;
      animation: pulse 1s infinite;
    }
    @keyframes pulse {
      0% { transform: scale(1); opacity: 0.7; }
      50% { transform: scale(1.3); opacity: 1; }
      100% { transform: scale(1); opacity: 0.7; }
    }

    /* Floating hearts background */
    .floating-heart {
      position: fixed;
      bottom: -50px;
      color: hotpink;
      font-size: 24px;
      animation: floatUp 8s linear infinite;
    }
    @keyframes floatUp {
      0% { transform: translateY(0) rotate(0deg); opacity: 1; }
      100% { transform: translateY(-100vh) rotate(360deg); opacity: 0; }
    }

    /* Final poem box */
    pre {
      background-color: #000;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 20px #ff4d4d;
      font-family: "Courier New", monospace;
      text-align: left;
      display: inline-block;
    }
  </style>
</head>
<body>
  <h1>💖 Unlock My Heart 💖</h1>

  <!-- Question 1 -->
  <div id="q1" class="question" style="display:block;">
    <p>What am I to you?</p>
    <button onclick="wrongAnswer()">Girlfriend</button>
    <button onclick="wrongAnswer()">Friend</button>
    <button onclick="checkAnswer(1)">Life Partner</button>
    <button onclick="wrongAnswer()">Either of them</button>
  </div>

  <!-- Question 2 -->
  <div id="q2" class="question">
    <p>What makes you impressed?</p>
    <button onclick="wrongAnswer()">My Smile</button>
    <button onclick="wrongAnswer()">My Eyes</button>
    <button onclick="wrongAnswer()">My Soul</button>
    <button onclick="wrongAnswer()">My Beauty</button>
    <button onclick="checkAnswer(2)">All of the above</button>
  </div>

  <!-- Question 3 -->
  <div id="q3" class="question">
    <p>What is my dream with you?</p>
    <button onclick="wrongAnswer()">Best future drama with you</button>
    <button onclick="wrongAnswer()">Having a kid with you</button>
    <button onclick="wrongAnswer()">Only giving torcher to you</button>
    <button onclick="checkAnswer(3)">Having lifetime healthy relationship with you</button>
  </div>

  <!-- Question 4 -->
  <div id="q4" class="question">
    <p>If I won't be on Earth one day, what will you do?</p>
    <button onclick="wrongAnswer()">Die for me</button>
    <button onclick="checkAnswer(4)">Take care of our baby</button>
    <button onclick="wrongAnswer()">Get depressed</button>
    <button onclick="wrongAnswer()">Live with someone else</button>
  </div>

  <!-- Question 5 -->
  <div id="q5" class="question">
    <p>What is the one thing you never want in our relationship?</p>
    <button onclick="wrongAnswer()">Cheating with someone else</button>
    <button onclick="wrongAnswer()">Bad wife behaviour</button>
    <button onclick="wrongAnswer()">Leaving you middle of the relationship</button>
    <button onclick="checkAnswer(5)">None of the above</button>
  </div>

  <!-- Question 6 -->
  <div id="q6" class="question">
    <p>What do you always want from me?</p>
    <button onclick="wrongAnswer()">Kiss</button>
    <button onclick="checkAnswer(6)">Hugs</button>
    <button onclick="wrongAnswer()">Romance</button>
    <button onclick="wrongAnswer()">S***x</button>
  </div>

  <!-- Question 7 -->
  <div id="q7" class="question">
    <p>If my beauty fades, will you still love me?</p>
    <button onclick="wrongAnswer()">You want beauty every time</button>
    <button onclick="wrongAnswer()">Are you ready to leave me</button>
    <button onclick="checkAnswer(7)">Ready to accept however I am</button>
    <button onclick="wrongAnswer()">Want me to change for yourself</button>
  </div>

  <!-- Question 8 -->
  <div id="q8" class="question">
    <p>If I make you angry, what will you do first?</p>
    <button onclick="wrongAnswer()">Bent for me</button>
    <button onclick="wrongAnswer()">Get angry too</button>
    <button onclick="wrongAnswer()">Don't try to fix it</button>
    <button onclick="checkAnswer(8)">Try to convince and spend more time with me</button>
  </div>

  <!-- Question 9 -->
  <div id="q9" class="question">
    <p>If you are in trouble, what kind of support do you want from me?</p>
    <button onclick="wrongAnswer()">Physically</button>
    <button onclick="wrongAnswer()">Emotionally</button>
    <button onclick="wrongAnswer()">Financially</button>
    <button onclick="checkAnswer(9)">All of the above</button>
  </div>

  <!-- Question 10 -->
  <div id="q10" class="question">
    <p>What do you like to call me always?</p>
    <button onclick="wrongAnswer()">Kanda</button>
    <button onclick="wrongAnswer()">Baby</button>
    <button onclick="checkAnswer(10)">Hendthi</button>
    <button onclick="wrongAnswer()">Chinna</button>
  </div>

  <!-- Question 11 -->
  <div id="q11" class="question">
    <p>If I'm in labour pain and doctor says only one can be saved, who would you choose?</p>
    <button onclick="checkAnswer(11)">Me (your partner)</button>
    <button onclick="wrongAnswer()">Baby</button>
    <button onclick="wrongAnswer()">Don't have answer for this</button>
    <button onclick="wrongAnswer()">Simply say I don't want them</button>
  </div>

  <!-- Final Screen -->
  <div id="final" class="question">
    <pre>
You are my <b>primary key</b>.
Every plan <b>references</b> you.
Every future <b>joins</b> on you.
Every query <b>expects</b> you.

Our tables will always exist,
every <b>record</b> will be complete.
Because without you, our
<b>relationships</b> just won't work.

SELECT * FROM forever;
INSERT INTO love VALUES ("eternally","endlessly");

<b style="color:#ff4d4d;">ERROR:</b> Foreign key constraint failed. ❤️
    </pre>
    <p style="color:pink; font-size:20px; margin-top:20px;">💞 From your lovely Hendthi 💞</p>
  </div>

  <script>
    function checkAnswer(q) {
      document.getElementById("q" + q).style.display = "none";
      if (q < 11) {
        document.getElementById("q" + (q + 1)).style.display = "block";
      } else {
        document.getElementById("final").style.display = "block";
      }
    }

    function wrongAnswer() {
      alert("😢 You don't understand your partner correctly...");
    }

    // Floating hearts generator
    function createHeart() {
      const heart = document.createElement("div");
      heart.className = "floating-heart";
      heart.innerHTML = "💖";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (5 + Math.random() * 5) + "
