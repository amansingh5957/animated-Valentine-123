<!DOCTYPE html>
<html>
<head>
  <title>Valentine 💖</title>
  <style>
    body {
      background: black;
      color: #ff4d6d;
      font-family: monospace;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    #box {
      font-size: 20px;
      white-space: pre-line;
      animation: glow 1s infinite alternate;
    }
    @keyframes glow {
      from { text-shadow: 0 0 5px #ff4d6d; }
      to { text-shadow: 0 0 20px #ff99aa; }
    }
  </style>
</head>
<body>
  <div id="box"></div>

  <script>
    const text = [
      "Initializing Love 💘",
      "Loading...",
      "█▒▒▒▒▒▒▒▒▒ 10%",
      "████▒▒▒▒▒▒ 40%",
      "███████▒▒▒ 80%",
      "██████████ 100%",
      "",
      "💖 I LOVE YOU 💖",
      "Happy Valentine’s Day 🌹"
    ];

    let i = 0;
    const box = document.getElementById("box");

    setInterval(() => {
      if (i < text.length) {
        box.innerHTML += text[i] + "\n";
        i++;
      }
    }, 700);
  </script>
</body>
</html>
