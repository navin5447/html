<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ISRO Farmer Helpbot</title>
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
      padding: 1.5rem 1rem;
    }
    header h1 {
      margin: 0;
      font-size: 1.8rem;
    }
    header p {
      margin: 0.5rem 0 0;
      font-size: 1rem;
    }
    main {
      max-width: 900px;
      margin: 2rem auto;
      padding: 0 1rem;
    }
    .chatbot-container {
      background: #ffffff;
      border-radius: 12px;
      padding: 1rem;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
    }
    iframe {
      width: 100%;
      height: 500px;
      border: none;
      border-radius: 10px;
    }
    .tips {
      margin-top: 1rem;
      font-size: 0.95rem;
      color: #444;
      background-color: #e0f2f1;
      padding: 0.75rem 1rem;
      border-radius: 8px;
      box-shadow: 0 1px 4px rgba(0, 0, 0, 0.05);
    }
    .quick-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-bottom: 1.5rem;
      margin-top: 1rem;
    }
    .quick-actions button {
      background-color: #4caf50;
      color: white;
      border: none;
      padding: 0.7rem 1.2rem;
      font-size: 0.95rem;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.2s ease;
    }
    .quick-actions button:hover {
      background-color: #388e3c;
    }
    .language-toggle {
      text-align: right;
      margin-top: -10px;
      margin-bottom: 20px;
    }
    .language-toggle button {
      background-color: #0288d1;
      color: white;
      border: none;
      padding: 0.5rem 1rem;
      border-radius: 6px;
      font-size: 0.9rem;
      cursor: pointer;
    }
    .language-toggle button:hover {
      background-color: #0277bd;
    }
  </style>
</head>
<body>

  <header>
    <h1>🌾 ISRO Farmer Helpbot</h1>
    <p>Ask about weather, soil, satellite data and farming tips</p>
  </header>

  <main>
    <div class="quick-actions">
      <button onclick="sendQuery('What is the weather forecast for my village?')">🌤 Weather</button>
      <button onclick="sendQuery('Show NDVI image for 635654')">🛰 NDVI</button>
      <button onclick="sendQuery('How to use Bhuvan map?')">🗺 Bhuvan Guide</button>
      <button onclick="sendQuery('Give me farming tips')">🌾 Farming Tips</button>
    </div>
    <div class="language-toggle">
      <button onclick="alert('Coming soon: Support for Hindi and Tamil')">🌐 Switch Language</button>
    </div>
    <div class="chatbot-container">
      <iframe src="https://console.dialogflow.com/api-client/demo/embedded/YOUR-BOT-ID-HERE" allow="microphone;"></iframe>
    </div>
    <div class="tips">
      💡 Try asking: "Will it rain in my village?" or "Show NDVI map for 635654"
    </div>

  </main>

  <script>
    function sendQuery(text) {
      alert("Sending query: " + text);
    }
  </script>

</body>
</html>
