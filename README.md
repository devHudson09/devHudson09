<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trio Lendário de Tecnologias</title>
    <!-- Inclui Tailwind CSS para estilização moderna e responsiva -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        /* Define a fonte Inter para todo o corpo */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #1a202c; /* Fundo escuro para contraste */
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px; /* Adiciona padding para telas menores */
            box-sizing: border-box;
        }

        /* Estilo para o contêiner principal do trio lendário */
        .legendary-trio-container {
            background: linear-gradient(135deg, #2d3748, #4a5568); /* Gradiente de fundo */
            padding: 2px; /* Espessura da borda "mágica" */
            border-radius: 1.5rem; /* Bordas arredondadas */
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05); /* Sombra sutil */
            max-width: 800px; /* Largura máxima para o quadro */
            width: 100%; /* Ocupa a largura total disponível */
            overflow: hidden; /* Garante que o brilho não vaze */
            position: relative;
        }

        /* Efeito de brilho da borda (similar ao quadro lendário) */
        .legendary-trio-container::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: conic-gradient(from 0deg at 50% 50%, #8b5cf6 0%, #ec4899 25%, #fcd34d 50%, #8b5cf6 75%, #ec4899 100%);
            animation: rotate 4s linear infinite; /* Animação de rotação do brilho */
            z-index: -1; /* Garante que o brilho fique atrás do conteúdo */
            opacity: 0.7; /* Transparência do brilho */
        }

        /* Animação de rotação para o brilho */
        @keyframes rotate {
            from {
                transform: rotate(0deg);
            }
            to {
                transform: rotate(360deg);
            }
        }

        /* Estilo para o conteúdo interno do trio */
        .legendary-trio-content {
            background-color: #2d3748; /* Cor de fundo do conteúdo */
            padding: 2.5rem; /* Espaçamento interno */
            border-radius: 1.5rem; /* Bordas arredondadas */
            color: #e2e8f0; /* Cor do texto */
            text-align: center;
            position: relative;
            z-index: 1;
        }

        /* Estilo para o título principal */
        .main-title {
            font-size: 2.5rem;
            font-weight: 700;
            color: #63b3ed;
            margin-bottom: 1.5rem;
            text-shadow: 0 0 10px rgba(99, 179, 237, 0.5);
        }

        /* Estilo para cada item de tecnologia */
        .tech-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 2rem;
            padding: 1.5rem;
            background-color: #4a5568; /* Fundo para cada item */
            border-radius: 1rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }

        .tech-item:hover {
            transform: translateY(-5px); /* Efeito de elevação no hover */
        }

        .tech-icon {
            margin-bottom: 1rem;
        }

        .tech-title {
            font-size: 1.75rem;
            font-weight: 600;
            color: #fcd34d; /* Cor dourada para títulos de tecnologia */
            margin-bottom: 0.5rem;
        }

        .tech-description {
            font-size: 1rem;
            color: #a0aec0;
            line-height: 1.5;
        }

        /* Responsividade para telas menores */
        @media (max-width: 768px) {
            .main-title {
                font-size: 2rem;
            }
            .tech-title {
                font-size: 1.5rem;
            }
            .tech-description {
                font-size: 0.9rem;
            }
            .legendary-trio-content {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="legendary-trio-container">
        <div class="legendary-trio-content">
            <h1 class="main-title">Os Guardiões do Meu Legado Digital! 🛡️✨</h1>

            <div class="mb-8">
                <img src="https://raw.githubusercontent.com/MicaelliMedeiros/micaellimedeiros/master/image/computer-ilustra.png" alt="Ilustração de um computador" class="mx-auto" width="300px"/>
            </div>

            <p class="text-lg text-gray-300 mb-8">
                Conheça a Tríade Sagrada da Web que Me Acompanha:
            </p>

            <!-- HTML Section -->
            <div class="tech-item">
                <div class="tech-icon">
                    <img align="center" alt="HTML5 Icon" height="50" width="60" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
                </div>
                <h3 class="tech-title">🏰 O Arquiteto Ancestral: HTML <span class="ml-2">🧱</span></h3>
                <p class="tech-description">
                    **O Mestre das Estruturas e Fundações.** Ele ergue os pilares de cada mundo digital, garantindo que a base seja sólida e imponente. Sem sua sabedoria, nenhuma história poderia ser contada na web.
                </p>
            </div>

            <!-- CSS Section -->
            <div class="tech-item">
                <div class="tech-icon">
                    <img align="center" alt="CSS3 Icon" height="50" width="60" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
                </div>
                <h3 class="tech-title">🎨 A Encanatadora Cromática: CSS <span class="ml-2">✨</span></h3>
                <p class="tech-description">
                    **A Feiticeira das Cores e Formas.** Ela dá vida e alma às estruturas, transformando meros contornos em paisagens vibrantes e interfaces deslumbrantes. Seus feitiços visuais são a magia que cativa os olhos dos exploradores.
                </p>
            </div>

            <!-- JavaScript Section -->
            <div class="tech-item">
                <div class="tech-icon">
                    <img align="center" alt="JavaScript Icon" height="50" width="60" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
                </div>
                <h3 class="tech-title">⚡ O Alquimista Dinâmico: JavaScript <span class="ml-2">🔮</span></h3>
                <p class="tech-description">
                    **O Conjurador de Interações e Magias.** Ele infunde movimento, inteligência e reatividade em cada canto, fazendo com que os mundos digitais respondam e se adaptem. Sua essência é a própria vida da experiência web.
                </p>
            </div>

            <p class="text-lg text-gray-300 mt-8">
                _Juntos, eles formam a base das minhas criações, transformando ideias em realidades que transcendem o comum. Prepare-se para testemunhar o poder desta aliança!_ 🚀
            </p>
        </div>
    </div>
</body>
</html>


# ✨ Bem-vindo(a) ao meu Domínio Digital! ✨

---

## 🚀 Sobre o Arquiteto por Trás do Código 🚀
Olá, Explorador(a) da Web! 👋 Eu sou um **Desenvolvedor Web Júnior** com uma paixão ardente por transformar ideias em experiências digitais incríveis. Cada linha de código é um passo em direção a um universo de possibilidades. Meu playground favorito? Onde **HTML**, **CSS** e **JavaScript** se encontram para criar magia! ✨

Estou sempre faminto por novos desafios e sedento por conhecimento, buscando oportunidades para codificar o futuro. Pronto para construir algo épico? 💻

---

## 🛠️ Meu Arsenal Tecnológico 🛠️

<div align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5 Badge"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3 Badge"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript Badge"/>
  <br><br>

  **HTML:** <span style="color: #E34F26;">████████████████████</span> (Nível Mestre! 🎯)
  <br>
  **CSS:** <span style="color: #1572B6;">████████████████████</span> (Estilizando o Universo! 🎨)
  <br>
  **JavaScript:** <span style="color: #F7DF1E; background-color: #333; padding: 2px 0;">████████████████████</span> (Lógica do Multiverso! 🧠)
  <br>
  <br>
</div>

---

## 🌐 Conecte-se e Vamos Codificar! 🌐
Minhas portas digitais estão sempre abertas para novas conexões, colaborações e brainstorms de ideias revolucionárias!
- 🚀 **GitHub:** [devHudson09](https://github.com/devHudson09) - Meu laboratório de projetos!
- 📧 **E-mail:** [devhudson.10@gmail.com](devhudson.10@gmail.com) (adicione seu email aqui) - Mande um sinal!
- 🔗 **LinkedIn:** [Hudson Santos]([https://linkedin.com/in/seu-perfil-linkedin](https://www.linkedin.com/in/hudson-santos-20a88b258/)) (adicione seu LinkedIn aqui) - Network de alta performance!

---

## 💡 Meus Projetos Estelares Recentes 💡
Uma amostra do que andei construindo em minha jornada:
- **`Projeto: Clone de Página Web`** 🌐: Uma réplica fiel, forjada em HTML e CSS, mostrando domínio da estrutura e estilo.
- **`Projeto: Interatividade com JavaScript`** 🕹️: Páginas que ganham vida! Demonstração de funções JavaScript para uma experiência dinâmica e envolvente.
- **`Projeto: Portfólio Online`** (EM CONSTRUÇÃO 🚧): Meu futuro epicentro de todas as criações, onde você poderá explorar meu universo de projetos!

---

## 🌟 Uma Mensagem do Coder 🌟
_Agradeço imensamente por explorar meu segmento digital! Vamos juntos programar o futuro e criar algo verdadeiramente **incrível e inovador**?_ 😊 Fico no aguardo de sua conexão!
