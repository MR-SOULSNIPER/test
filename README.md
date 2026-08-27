<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GTA Experience</title>

<style>
    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-family: Arial, sans-serif;
    }

    body {
        min-height: 100vh;
        background: linear-gradient(135deg, #111, #222, #000);
        color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
    }

    .page {
        width: 90%;
        max-width: 850px;
        padding: 40px;
        background: rgba(0,0,0,0.75);
        border-radius: 20px;
        box-shadow: 0 0 30px rgba(255,255,255,0.15);
    }

    h1 {
        font-size: 45px;
        margin-bottom: 20px;
        color: #f5c400;
    }

    h2 {
        font-size: 32px;
        margin-bottom: 20px;
        color: #f5c400;
    }

    p {
        font-size: 18px;
        line-height: 1.7;
        margin-bottom: 25px;
        color: #ddd;
    }

    input {
        width: 80%;
        padding: 15px;
        border-radius: 10px;
        border: none;
        outline: none;
        font-size: 18px;
        text-align: center;
        margin-bottom: 15px;
    }

    button {
        width: 80%;
        padding: 16px;
        border: none;
        border-radius: 12px;
        background: #f5c400;
        color: black;
        font-size: 20px;
        font-weight: bold;
        cursor: pointer;
        transition: 0.3s;
    }

    button:hover {
        transform: scale(1.05);
        background: #ffdd33;
    }

    .hidden {
        display: none;
    }

    .error {
        color: #ff4444;
        margin-top: 10px;
        font-weight: bold;
    }
</style>
</head>

<body>

<!-- PASSWORD PAGE -->
<div class="page" id="passwordPage">

    <h1>🎮 GTA EXPERIENCE 🎮</h1>

    <p>
        Welcome to the GTA experience.<br>
        Enter the secret password to continue.
    </p>

    <input type="password" id="password" placeholder="Enter password">

    <button onclick="checkPassword()">ENTER GTA</button>

    <div class="error" id="error"></div>

</div>


<!-- PAGE 1 -->
<div class="page hidden" id="page1">

    <h2>🔥 Welcome to GTA 🔥</h2>

    <p>
        Grand Theft Auto is one of the most famous open-world
        game series ever created. GTA lets you explore huge cities,
        drive cars, complete missions, meet different characters
        and create your own crazy adventures.
    </p>

    <button onclick="nextPage(2)">NEXT ➜</button>

</div>


<!-- PAGE 2 -->
<div class="page hidden" id="page2">

    <h2>🚗 The GTA World</h2>

    <p>
        In GTA, the world is filled with cars, bikes, planes,
        boats, weapons, missions and activities. You can drive
        around the city, take part in races, complete missions
        or simply cause chaos and explore the map.
    </p>

    <button onclick="nextPage(3)">NEXT ➜</button>

</div>


<!-- PAGE 3 -->
<div class="page hidden" id="page3">

    <h2>💰 Missions & Adventures</h2>

    <p>
        GTA gives you missions where you can work with different
        characters, make money and unlock new parts of the game.
        Some missions are serious, while others are completely crazy.
    </p>

    <button onclick="nextPage(4)">NEXT ➜</button>

</div>


<!-- PAGE 4 -->
<div class="page hidden" id="page4">

    <h2>🌆 The Open World</h2>

    <p>
        One of the best things about GTA is the freedom.
        You can choose what you want to do. Explore the city,
        customize vehicles, discover hidden locations and
        experience the world in your own way.
    </p>

    <button onclick="nextPage(5)">NEXT ➜</button>

</div>


<!-- FINAL PAGE -->
<div class="page hidden" id="page5">

    <h1>🎮 GTA 🎮</h1>

    <p>
        The world of GTA is about freedom, adventure,
        crazy moments and unforgettable stories.
        There is always something waiting around the next corner.
    </p>

    <button onclick="location.reload()">PLAY AGAIN 🔄</button>

</div>


<script>

function checkPassword() {

    const password = document.getElementById("password").value;
    const error = document.getElementById("error");

    if (password === "0333") {

        document.getElementById("passwordPage").classList.add("hidden");
        document.getElementById("page1").classList.remove("hidden");

    } else {

        error.innerText = "❌ Wrong password. Try again.";

    }
}


function nextPage(pageNumber) {

    document.querySelectorAll(".page").forEach(page => {
        page.classList.add("hidden");
    });

    document.getElementById("page" + pageNumber).classList.remove("hidden");

}

</script>

</body>
</html>
