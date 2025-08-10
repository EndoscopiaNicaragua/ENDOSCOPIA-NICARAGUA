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
      gap: 10px;
    }
    .panel li img.video-icon {
      width: 24px;
      height: 24px;
      filter: invert(1);
    }
    .panel li a {
      color: #aad4ff;
      text-decoration: none;
      font-weight: 500;
      font-size: 1rem;
    }
    .panel li a:hover {
      text-decoration: underline;
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
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=y2L6iQK8HEM" target="_blank" rel="noopener noreferrer">Angiodisplasia gástrica</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=6MjwMITIQfM" target="_blank" rel="noopener noreferrer">Varices esofágicas de gran tamaño</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=mou-UHDCUrg" target="_blank" rel="noopener noreferrer">Tumor de píloro</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=-4vMUr155T8" target="_blank" rel="noopener noreferrer">Divertículo duodenal</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=a5dnIREZ8zU" target="_blank" rel="noopener noreferrer">Pangastritis hemorrágica</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=cagaqoffQNY" target="_blank" rel="noopener noreferrer">Hernia deslizante</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=wwSWdHh1fTI" target="_blank" rel="noopener noreferrer">Gastritis erosiva</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=YdjVDeQroKk" target="_blank" rel="noopener noreferrer">Polipectomía gástrica</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=k0fO2Jx46pQ" target="_blank" rel="noopener noreferrer">Esofagitis</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=5hn7w2qk1RI" target="_blank" rel="noopener noreferrer">Poliposis gástrica</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=2-mSh50Jwsw" target="_blank" rel="noopener noreferrer">Tumor de cuerpo gástrico</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=8NZZPkzEEx0" target="_blank" rel="noopener noreferrer">Prolapso gástrico</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=Ws3NdY_R8nc" target="_blank" rel="noopener noreferrer">Pangastritis hipertensiva</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=wBRnQGNPB5w" target="_blank" rel="noopener noreferrer">Cuerpo extraño hueso en esófago</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/watch?v=cN9uSHL1VMc" target="_blank" rel="noopener noreferrer">Cuerpo extraño trozo de carne de hace 5 días en esófago</a></li>
      </ul>
    </div>

    <button class="accordion">
      <img class="icon" src="https://img.icons8.com/ios-filled/50/ffffff/colon.png" alt="Icono Colonoscopia"/>
      Colonoscopía
    </button>
    <div class="panel">
      <ul>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://www.youtube.com/shorts/L1biKnBI2NY" target="_blank" rel="noopener noreferrer">Diverticulosis</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://youtube.com/shorts/51X-pwj61Zk" target="_blank" rel="noopener noreferrer">Colonoscopía normal</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://youtube.com/shorts/Udg3Fxi0u4c" target="_blank" rel="noopener noreferrer">Triocéfalo</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://youtube.com/shorts/rXtSRnQTsug" target="_blank" rel="noopener noreferrer">Pólipo en recto</a></li>
        <li><img class="video-icon" src="https://img.icons8.com/ios-filled/50/ffffff/video.png" alt="Video icon"/><a href="https://youtu.be/eU0maFhLuwA" target="_blank" rel="noopener noreferrer">Tumor de recto</a></li>
      </ul>
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
  </script>
</body>
</html>
