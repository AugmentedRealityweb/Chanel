<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body, html {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden; /* Previne scroll-ul dacă nu este necesar */
    }
    model-viewer {
      width: 100%; /* Folosește întreaga lățime disponibilă */
      height: 100%; /* Folosește întreaga înălțime disponibilă */
    }
    .ar-button {
      padding: 10px 20px;
      background-color: #007BFF;
      border: none;
      border-radius: 5px;
      color: white;
      cursor: pointer;
      transition: background-color 0.3s, box-shadow 0.3s;
    }
    .ar-button:hover {
      background-color: #0056b3;
    }
  </style>
  <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
</head>
<body>
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
</body>
</html>
