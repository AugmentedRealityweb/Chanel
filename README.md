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
