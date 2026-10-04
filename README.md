# index.html-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Nibhul OS Prototype</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #0a0f1c;
      color: #e0f7ff;
    }
    header {
      text-align: center;
      padding: 20px;
      background: linear-gradient(90deg, #0a0f1c, #0f1f3a);
      border-bottom: 1px solid cyan;
    }
    header h1 {
      color: cyan;
      text-shadow: 0 0 10px cyan;
    }
    header p {
      color: #fff;
      font-size: 14px;
    }
    .dashboard {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
      padding: 20px;
    }
    .card {
      background: rgba(20, 30, 50, 0.8);
      border: 1px solid cyan;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 0 15px rgba(0,255,255,0.3);
      transition: transform 0.3s;
    }
    .card:hover {
      transform: scale(1.05);
      box-shadow: 0 0 25px cyan;
    }
    .card h2 {
      color: cyan;
      margin-bottom: 10px;
    }
    .tasks ul {
      list-style: none;
      padding: 0;
    }
    .tasks li {
      margin: 5px 0;
      padding: 5px;
      border-bottom: 1px solid #444;
    }
    .voice {
      text-align: center;
    }
    .waveform {
      width: 100%;
      height: 50px;
      background: repeating-linear-gradient(
        to right,
        cyan 0px,
        cyan 2px,
        transparent 2px,
        transparent 4px
      );
      animation: pulse 1s infinite;
    }
    @keyframes pulse {
      0% { opacity: 0.3; }
      50% { opacity: 1; }
      100% { opacity: 0.3; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Nibhul OS</h1>
    <p>FutureNest • SafeDisha • Personal Agentic AI</p>
  </header>
  
  <div class="dashboard">
    <div class="card">
      <h2>FutureNest Smart Home</h2>
      <p>Home Automation & Control</p>
    </div>
    <div class="card">
      <h2>SafeDisha Dashboard</h2>
      <p>AI Security & Analytics</p>
    </div>
    <div class="card">
      <h2>AI Identity Hub</h2>
      <p>Secure Digital Identity</p>
    </div>
    <div class="card">
      <h2>Health Sync</h2>
      <p>Health Monitoring</p>
    </div>
    <div class="card">
      <h2>Finance Manager</h2>
      <p>Balance: $12,680</p>
    </div>
    <div class="card voice">
      <h2>Voice Assistant</h2>
      <div class="waveform"></div>
      <p>How can I assist you today?</p>
    </div>
    <div class="card tasks">
      <h2>Upcoming Tasks</h2>
      <ul>
        <li>2:00 PM Meeting with Team</li>
        <li>4:30 PM Gym Session</li>
        <li>7:00 PM Home Security Check</li>
      </ul>
    </div>
  </div>
</body>
</html>
