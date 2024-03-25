<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background-image: url('fundal6.jpg');
      background-size: cover;
      background-position: center;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 90vh;
    }
    .model-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      margin-top: 220px;
    }
    .model-section, .iframe-section {
      text-align: center;
      margin-bottom: 20px;
    }
    model-viewer, iframe {
      width: 300px; /* Adjusted for consistency */
      height: 400px; /* Adjusted for consistency */
      margin: 0 auto;
      border-radius: 20px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    .ar-button {
      padding: 10px 15px;
      font-size: 0.9rem;
      margin-top: 10px;
      background-color: #007BFF;
      border: none;
      border-radius: 20px;
      color: white;
      cursor: pointer;
      transition: background-color 0.3s, box-shadow 0.3s;
    }
    .ar-button:hover {
      background-color: #0056b3;
    }
    .back-link {
      display: block;
      margin-top: 20px;
      text-decoration: none;
      color: white;
      background-color: #007BFF;
      padding: 10px 15px;
      border-radius: 20px;
      font-size: 0.9rem;
      transition: background-color 0.3s;
    }
    .back-link:hover {
      background-color: #0056b3;
    }
  </style>
  <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
</head>
<body>
<div class="model-container">
  <div class="model-section">
    <model-viewer
      src="bag.glb"
      ios-src="bag.usdz"
      ar
      ar-modes="webxr scene-viewer quick-look"
      camera-controls
      auto-rotate
      environment-image="neutral"
      shadow-intensity="1"
      loading="lazy"
      alt="Bag"
      min-camera-orbit="auto 0deg 0deg"
      max-camera-orbit="auto 80deg auto">
      <button slot="ar-button" class="ar-button">Activează modul AR</button>
    </model-viewer>
  </div>
  <div class="iframe-section">
    <iframe width="100%" height="100%" frameborder="0" allowfullscreen src="https://scaniverse.com/scan/k6oq3xbrrsll4ahe?embed=1"></iframe>
    <!-- Assuming the platform supports direct AR activation, this button might help -->
    <button onclick="window.open('https://scaniverse.com/scan/k6oq3xbrrsll4ahe', '_blank');" class="ar-button">Vezi în modul AR</button>
  </div>
  <a href="https://www.titi-valenti.ro/setul-duo-chic-black.html" class="back-link">Înapoi la pagină produs</a>
</div>
</body>
