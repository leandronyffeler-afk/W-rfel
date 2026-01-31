<!doctype html>
<html lang="de">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Würfel</title>
  <style>
    body {
      font-family: system-ui, Arial, sans-serif;
      max-width: 420px;
      margin: 40px auto;
      padding: 0 16px;
      text-align: center;
    }
    button {
      width: 100%;
      padding: 20px;
      margin-top: 20px;
      font-size: 24px;
      cursor: pointer;
      border-radius: 16px;
      border: 1px solid #ccc;
    }
    .result {
      margin-top: 30px;
      font-size: 48px;
      font-weight: 900;
    }
  </style>
</head>
<body>
  <h1>🎲 Würfel</h1>
  <p>Einfacher Würfel von 1–6</p>

  <button onclick="würfeln()">Würfeln</button>

  <div id="anzeige" class="result">–</div>

  <script>
    function würfeln() {
      const zahl = Math.floor(Math.random() * 6) + 1;
      document.getElementById("anzeige").textContent = zahl;
    }
  </script>
</body>
</html>
