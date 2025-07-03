

<!DOCTYPE html>
<html lang="en">
<head>
   <link rel="stylesheet" href="style.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ISRO Farmer Helpbot</title>
   <div style="text-align:right; margin-top: 10px;">
  <button onclick="alert('Coming soon: Hindi / Tamil support')">🌐 Switch Language</button>
</div>
   <img src="assets/weather-icon.png" alt="Weather" width="32">
    <style>
        body {
  font-family: Arial, sans-serif;
  background-color: #eef6f2;
  margin: 0;
  padding: 0;
}

header {
  background-color: #2e7d32;
  color: white;
  text-align: center;
  padding: 1rem;
  font-size: 1.2rem;
}

main {
  max-width: 900px;
  margin: auto;
  padding: 2rem;
}

.chatbot-container {
  background: #fff;
  border-radius: 12px;
  padding: 1rem;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

iframe {
  width: 100%;
  height: 500px;
  border: none;
  border-radius: 8px;
}
tips {
            margin-top: 1rem;
            font-size: 0.95rem;
            color: #666;
        }
    </style>
</head>
<body>

<header>
    <h1>🌾 ISRO Farmer Helpbot</h1>
    <p>Get weather, soil, satellite and farming info in one chat</p>
</header>

<main>
    <div class="chatbot">
        <!-- Replace this iframe with your Dialogflow or custom bot -->
<iframe src="https://console.dialogflow.com/api-client/demo/embedded/YOUR-BOT-ID-HERE"></iframe>
        <div class="tips">
            Tip: Try asking “Will it rain in my village?” or “Show me NDVI image for pincode 635654”
        </div>
    </div>
</main>

</body>
</html>

