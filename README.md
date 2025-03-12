<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bem-vindo(a) ao meu perfil</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(120deg, #3498db, #8e44ad);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      color: white;
    }
    .bio-container {
      text-align: center;
      padding: 20px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 10px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
      animation: slideIn 1.5s ease-in-out;
    }
    .bio-container h1 {
      font-size: 2.5rem;
      color: #f1c40f;
      margin-bottom: 10px;
    }
    .bio-container p {
      font-size: 1.2rem;
      line-height: 1.8;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.2);
    }
    .icons {
      display: inline-flex;
      gap: 15px;
      margin-top: 15px;
    }
    .icons img {
      width: 40px;
      height: 40px;
      transition: transform 0.3s ease;
    }
    .icons img:hover {
      transform: scale(1.2);
    }
    @keyframes slideIn {
      0% {
        transform: translateY(-20px);
        opacity: 0;
      }
      100% {
        transform: translateY(0);
        opacity: 1;
      }
    }
  </style>
</head>
<body>
  <div class="bio-container">
    <h1>Bem-vindo(a) ao meu perfil 😁</h1>
    <p>Sou um Desenvolvedor Web Júnior buscando por experiências incríveis na web. Trabalhando com HTML, CSS e JavaScript para transformar ideias em realidade.</p>
    <div class="icons">
      <a href="https://github.com/devHudson09" target="_blank">
        <img alt="GitHub" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/github/github-original.svg">
      </a>
      <img alt="JavaScript" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
      <img alt="HTML5" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
      <img alt="CSS3" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
    </div>
  </div>
</body>
</html>
