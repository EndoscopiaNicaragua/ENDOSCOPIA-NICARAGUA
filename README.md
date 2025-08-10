<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Centro Nacional de Endoscopía</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #001f3f; /* Navy */
    color: white;
    margin: 0;
    padding: 0;
    text-align: center;
  }
  header {
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    padding: 10px;
    background-color: #001a33;
  }
  header img {
    position: absolute;
    left: 10px;
    top: 10px;
    width: 60px;
    height: auto;
  }
  h1 {
    margin: 0;
    font-size: 28px;
  }
  .search-box {
    margin: 20px 0;
  }
  .search-box input {
    padding: 5px;
    font-size: 14px;
    width: 250px;
  }
  .gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 20px;
  }
  .video-card {
    background-color: #003366;
    padding: 10px;
    border-radius: 10px;
  }
  iframe {
    width: 100%;
    height: 150px;
    border-radius: 8px;
  }
  h3 {
    font-size: 14px;
    margin: 8px 0 0;
  }
</style>
<script>
function buscarVideos() {
  let input = document.getElementById('buscar').value.toLowerCase();
  let videos = document.getElementsByClassName('video-card');
  for (let i = 0; i < videos.length; i++) {
    let titulo = videos[i].getElementsByTagName('h3')[0].innerText.toLowerCase();
    videos[i].style.display = titulo.includes(input) ? '' : 'none';
  }
}
</script>
</head>
<body>
<header>
  <img src="logo.png" alt="Logo Centro Nacional de Endoscopía">
  <h1>Centro Nacional de Endoscopía</h1>
</header>
<div class="search-box">
  <input type="text" id="buscar" onkeyup="buscarVideos()" placeholder="Buscar videos...">
</div>
<h2>Endoscopia Digestiva Alta</h2>
<div class="gallery">
  <div class="video-card">
    <iframe src="https://www.youtube.com/embed/hEHM_PFZZo0" frameborder="0" allowfullscreen></iframe>
    <h3>Video de Endoscopia 1</h3>
  </div>
</div>
<h2>Colonoscopia</h2>
<div class="gallery">
  <div class="video-card">
    <iframe src="https://www.youtube.com/embed/XEepqhqNZtQ" frameborder="0" allowfullscreen></iframe>
    <h3>Video de Colonoscopia 1</h3>
  </div>
</div>
</body>
</html>
