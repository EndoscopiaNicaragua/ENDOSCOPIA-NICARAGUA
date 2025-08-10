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
    }
    header img {
      height: 60px;
      margin-right: 20px;
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
        <li data-video="6MjwMITIQfM">
          <img class="video-icon" src="https://img.youtube.com/vi/6MjwMITIQfM/hqdefault.jpg" alt="Varices esofágicas de gran tamaño"/>
          <span>Varices esofágicas de gran tamaño</span>
        </li>
        <li data-video="mou-UHDCUrg">
          <img class="video-icon" src="https://img.youtube.com/vi/mou-UHDCUrg/hqdefault.jpg" alt="Tumor de píloro"/>
          <span>Tumor de píloro</span>
        </li>
        <li data-video="-4vMUr155T8">
          <img class="video-icon" src="https://img.youtube.com/vi/-4vMUr155T8/hqdefault.jpg" alt="Divertículo duodenal"/>
          <span>Divertículo duodenal</span>
        </li>
        <li data-video="a5dnIREZ8zU">
          <img class="video-icon" src="https://img.youtube.com/vi/a5dnIREZ8zU/hqdefault.jpg" alt="Pangastritis hemorrágica"/>
          <span>Pangastritis hemorrágica</span>
        </li>
        <li data-video="cagaqoffQNY">
          <img class="video-icon" src="https://img.youtube.com/vi/cagaqoffQNY/hqdefault.jpg" alt="Hernia deslizante"/>
          <span>Hernia deslizante</span>
        </li>
        <li data-video="wwSWdHh1fTI">
          <img class="video-icon" src="https://img.youtube.com/vi/wwSWdHh1fTI/hqdefault.jpg" alt="Gastritis erosiva"/>
          <span>Gastritis erosiva</span>
        </li>
        <li data-video="YdjVDeQroKk">
          <img class="video-icon" src="https://img.youtube.com/vi/YdjVDeQroKk/hqdefault.jpg" alt="Polipectomía gástrica"/>
          <span>Polipectomía gástrica</span>
        </li>
        <li data-video="k0fO2Jx46pQ">
          <img class="video-icon" src="https://img.youtube.com/vi/k0fO2Jx46pQ/hqdefault.jpg" alt="Esofagitis"/>
          <span>Esofagitis</span>
        </li>
        <li data-video="5hn7w2qk1RI">
          <img class="video-icon" src="https://img.youtube.com/vi/5hn7w2qk1RI/hqdefault.jpg" alt="Poliposis gástrica"/>
          <span>Poliposis gástrica</span>
        </li>
        <li data-video="2-mSh50Jwsw">
          <img class="video-icon" src="https://img.youtube.com/vi/2-mSh50Jwsw/hqdefault.jpg" alt="Tumor de cuerpo gástrico"/>
          <span>Tumor de cuerpo gástrico</span>
        </li>
        <li data-video="8NZZPkzEEx0">
          <img class="video-icon" src="https://img.youtube.com/vi/8NZZPkzEEx0/hqdefault.jpg" alt="Prolapso gástrico"/>
          <span>Prolapso gástrico</span>
        </li>
        <li data-video="Ws3NdY_R8nc">
          <img class="video-icon" src="https://img.youtube.com/vi/Ws3NdY_R8nc/hqdefault.jpg" alt="Pangastritis hipertensiva"/>
          <span>Pangastritis hipertensiva</span>
        </li>
        <li data-video="wBRnQGNPB5w">
          <img class="video-icon" src="https://img.youtube.com/vi/wBRnQGNPB5w/hqdefault.jpg" alt="Cuerpo extraño hueso en esófago"/>
          <span>Cuerpo extraño hueso en esófago</span>
        </li>
        <li data-video="cN9uSHL1VMc">
          <img class="video-icon" src="https://img.youtube.com/vi/cN9uSHL1VMc/hqdefault.jpg" alt="Cuerpo extraño trozo de carne de hace 5 días en esófago"/>
          <span>Cuerpo extraño trozo de carne de hace 5 días en esófago</span>
        </li>
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
        <li data-video="51X-pwj61Zk">
          <img class="video-icon" src="https://img.youtube.com/vi/51X-pwj61Zk/hqdefault.jpg" alt="Colonoscopía normal"/>
          <span>Colonoscopía normal</span>
        </li>
        <li data-video="Udg3Fxi0u4c">
          <img class="video-icon" src="https://img.youtube.com/vi/Udg3Fxi0u4c/hqdefault.jpg" alt="Triocéfalo"/>
          <span>Triocéfalo</span>
        </li>
        <li data-video="rXtSRnQTsug">
          <img class="video-icon" src="https://img.youtube.com/vi/rXtSRnQTsug/hqdefault.jpg" alt="Pólipo en recto"/>
          <span>Pólipo en recto</span>
        </li>
        <li data-video="eU0maFhLuwA">
          <img class="video-icon" src="https://img.youtube.com/vi/eU0maFhLuwA/hqdefault.jpg" alt="Tumor de recto"/>
          <span>Tumor de recto</span>
        </li>
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
