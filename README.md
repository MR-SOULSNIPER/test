<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Angel ❤️</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <style>
    body {
      margin: 0;
      min-height: 100vh;
      background: linear-gradient(#ffb6c1, #ffe4e1);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: "Comic Sans MS", cursive, sans-serif;
    }

    .page {
      display: none;
      text-align: center;
      max-width: 360px;
      padding: 20px;
    }

    .page.active {
      display: block;
    }

    .paper {
      background: white;
      padding: 26px;
      border-radius: 14px;
      box-shadow: 0 10px 20px rgba(0,0,0,0.25);
      margin-bottom: 10px;
    }

    .paper h1 {
      color: #e75480;
      font-size: 24px;
      margin-bottom: 12px;
    }

    .paper p {
      color: #444;
      font-size: 16px;
      line-height: 1.6;
    }

    .bear {
      font-size: 150px;
      margin-top: 5px;
    }

    button {
      margin-top: 18px;
      padding: 10px 22px;
      border: none;
      border-radius: 20px;
      background: #ff69b4;
      color: white;
      font-size: 14px;
      cursor: pointer;
    }

    button:hover {
      background: #ff1493;
    }
  </style>
</head>

<body>

  <!-- PAGE 1 -->
  <div class="page active">
    <div class="paper">
      <h1>Angel ❤️</h1>
      <p>
        I made this just for you.<br><br>
        Every word you’re about to read
        comes straight from my heart.
      </p>
      <button onclick="nextPage()">Next</button>
    </div>
    <div class="bear">🧸</div>
  </div>

  <!-- PAGE 2 -->
  <div class="page">
    <div class="paper">
      <p>
        You mean more to me than I ever knew
        how to put into words.<br><br>
        You didn’t just become important to me —
        you became a part of me.
      </p>
      <button onclick="nextPage()">Next</button>
    </div>
    <div class="bear">🧸</div>
  </div>

  <!-- PAGE 3 -->
  <div class="page">
    <div class="paper">
      <p>
        When things feel heavy,
        you make them feel lighter.<br><br>
        Your presence alone brings me comfort,
        peace, and strength.
      </p>
      <button onclick="nextPage()">Next</button>
    </div>
    <div class="bear">🧸</div>
  </div>

  <!-- PAGE 4 -->
  <div class="page">
    <div class="paper">
      <p>
        Your smile stays in my thoughts.<br>
        Your voice stays in my heart.<br><br>
        No matter where I am,
        I carry you with me.
      </p>
      <button onclick="nextPage()">Next</button>
    </div>
    <div class="bear">🧸</div>
  </div>

  <!-- PAGE 5 -->
  <div class="page">
    <div class="paper">
      <p>
        You make me feel seen.<br>
        You make me feel understood.<br>
        You make me feel loved.<br><br>
        And that means everything to me.
      </p>
      <button onclick="nextPage()">Next</button>
    </div>
    <div class="bear">🧸</div>
  </div>

  <!-- PAGE 6 -->
  <div class="page">
    <div class="paper">
      <h1>My Angel 💖</h1>
      <p>
        I care about you deeply.<br>
        I believe in you.<br>
        And I’m so grateful for you.<br><br>
        My heart will always choose you.
      </p>
    </div>
    <div class="bear">🧸❤️</div>
  </div>

  <script>
    let currentPage = 0;
    const pages = document.querySelectorAll(".page");

    function nextPage() {
      pages[currentPage].classList.remove("active");
      currentPage++;
      pages[currentPage].classList.add("active");
    }
  </script>

</body>
</html>
