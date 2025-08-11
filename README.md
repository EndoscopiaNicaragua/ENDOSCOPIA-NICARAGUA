<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Centro Nacional de Endoscopia</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #001f3f; /* azul navy */
      color: white;
    }
    header {
      background-color: #001f3f;
      padding: 15px 30px;
      display: flex;
      align-items: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.5);
      gap: 15px;
    }
    header img {
      height: 80px;
      width: auto;
    }
    header h1 {
      margin: 0;
      font-size: 1.8rem;
      font-weight: bold;
    }
    main {
      padding: 20px 30px;
      max-width: 900px;
      margin: auto;
    }
    h2 {
      margin-top: 0;
      border-bottom: 2px solid white;
      padding-bottom: 10px;
    }
    /* Acordeón */
    .accordion {
      background-color: #003366;
      color: white;
      cursor: pointer;
      padding: 15px 20px;
      width: 100%;
      border: none;
      text-align: left;
      outline: none;
      font-size: 1.2rem;
      display: flex;
      align-items: center;
      gap: 10px;
      border-radius: 6px;
      margin-bottom: 10px;
      user-select: none;
      transition: background-color 0.3s ease;
    }
    .accordion:hover {
      background-color: #00509e;
    }
    .accordion img.icon {
      width: 30px;
      height: 30px;
    }
    .accordion:after {
      content: '\25BC'; /* flecha hacia abajo */
      margin-left: auto;
      transition: transform 0.3s ease;
    }
    .accordion.active:after {
      transform: rotate(180deg); /* flecha hacia arriba */
    }
    .panel {
      background-color: #002147;
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.4s ease;
      border-radius: 0 0 6px 6px;
      padding-left: 20px;
      margin-bottom: 20px;
    }
    .panel ul {
      list-style: none;
      padding: 0;
      margin: 10px 0;
    }
    .panel li {
      margin: 8px 0;
      display: flex;
      align-items: center;
      gap: 15px;
      cursor: pointer;
    }
    .panel li img.video-icon {
      width: 120px;  /* miniatura más grande */
      height: 90px;
      border-radius: 6px;
      object-fit: cover;
      pointer-events: none;
    }
    .panel li span {
      color: #aad4ff;
      font-weight: 600;
      font-size: 1.2rem;  /* letra más grande */
      user-select: none;
    }
    .panel li:hover span {
      text-decoration: underline;
    }
    #video-player {
      margin-top: 30px;
      background: #002147;
      border-radius: 8px;
      padding: 10px;
      display: flex;
      justify-content: center;
    }
    #video-player iframe {
      width: 100%;
      max-width: 800px;
      height: 450px;
      border: none;
      border-radius: 6px;
    }
  </style>
</head>
<body>
  <header>
    <img src="images/logo.png" alt="Logo Centro Nacional de Endoscopia" />
    <h1>Centro Nacional de Endoscopia</h1>
  </header>

  <main>
    <button class="accordion">
      <img class="icon" src="https://img.icons8.com/ios-filled/50/ffffff/stomach.png" alt="Icono Endoscopia Digestiva Alta"/>
      Endoscopía Digestiva Alta
    </button>
    <div class="panel">
      <ul>
        <li data-video="y2L6iQK8HEM">
          <img class="video-icon" src="https://img.youtube.com/vi/y2L6iQK8HEM/hqdefault.jpg" alt="Angiodisplasia gástrica"/>
          <span>Angiodisplasia gástrica</span>
        </li>
        <!-- Los demás videos iguales -->
      </ul>
    </div>

    <button class="accordion">
      <img class="icon" src="https://img.icons8.com/ios-filled/50/ffffff/colon.png" alt="Icono Colonoscopia"/>
      Colonoscopía
    </button>
    <div class="panel">
      <ul>
        <li data-video="L1biKnBI2NY">
          <img class="video-icon" src="https://img.youtube.com/vi/L1biKnBI2NY/hqdefault.jpg" alt="Diverticulosis"/>
          <span>Diverticulosis</span>
        </li>
        <!-- Los demás videos iguales -->
      </ul>
    </div>

    <div id="video-player">
      <p>Selecciona un video para reproducirlo aquí.</p>
    </div>
  </main>

  <script>
    const accordions = document.querySelectorAll('.accordion');
    accordions.forEach(button => {
      button.addEventListener('click', () => {
        button.classList.toggle('active');
        const panel = button.nextElementSibling;
        if(panel.style.maxHeight){
          panel.style.maxHeight = null;
        } else {
          panel.style.maxHeight = panel.scrollHeight + "px";
        }
      });
    });

    const videoPlayer = document.getElementById('video-player');
    const videoItems = document.querySelectorAll('.panel li');

    videoItems.forEach(item => {
      item.addEventListener('click', () => {
        const videoId = item.getAttribute('data-video');
        if(videoId) {
          videoPlayer.innerHTML = `<iframe src="https://www.youtube.com/embed/${videoId}" allowfullscreen allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe>`;
          videoPlayer.scrollIntoView({behavior: "smooth"});
        }
      });
    });
  </script>
</body>
</html>
