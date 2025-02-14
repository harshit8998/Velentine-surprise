# Velentine-surprise<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Special Valentine Surprise 💖</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1 id="message">I Have a Surprise for You! 🎁</h1>
        <button onclick="showSurprise()">💖 Tap to Reveal 💖</button>
        <p id="finalMessage" style="display: none;">You Are My Forever Valentine! ❤️</p>
    </div>
    
    <audio id="loveSong" src="valentine-song.mp3"></audio>
    
    <script src="script.js"></script>
</body>
</html>
body {
    text-align: center;
    background-color: black;
    color: white;
    font-family: Arial, sans-serif;
    transition: background 2s, color 2s;
}

.container {
    margin-top: 20%;
}

button {
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    background: red;
    color: white;
    cursor: pointer;
    border-radius: 10px;
    margin-top: 20px;
}

button:hover {
    background: darkred;
}
function showSurprise() {
    document.body.style.backgroundColor = "pink";
    document.body.style.color = "black";
    document.getElementById("message").style.display = "none";
    document.getElementById("finalMessage").style.display = "block";
    document.getElementById("loveSong").play();
}
