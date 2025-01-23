<head>
<style>
body {margin: 0; font-family: 'Arial', sans-serif;  background-color: #f7f7f7;  color: #333;}
.profile-container { max-width: 1200px;  margin: 0 auto;  padding: 20px; }
.navbar { display: flex;  justify-content: space-between;  align-items: center;  background-color: #000; padding: 15px 30px; border-radius: 10px; }
.navbar ul {list-style: none; display: flex; gap: 15px;}
.navbar li a { text-decoration: none; color: white; font-weight: bold; cursor: pointer;}
.active { text-decoration: darkgrey;}
.section { display: none; margin-top: 40px;  background-color: white; padding: 30px; border-radius: 15px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); }
.section.active {display: block; }
.tags {margin-top: 20px; }
.tags img {margin-right: 10px; vertical-align: middle;}
.profile-photo { text-align: center; margin-top: 20px; }
.profile-photo img { width: 200px; height: 200px; border-radius: 50%; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);}
</style>
</head>

<body>
<div class="profile-container">
    
<header>
<nav class="navbar"> 
<ul>
<li><a data-section="about" class="nav-link active">À propos</a></li>
<li><a data-section="experience" class="nav-link">Expériences</a></li>
<li><a data-section="projects" class="nav-link">Projets</a></li>
</ul>
</nav>
</header>

<section id="about" class="section active">

<div class="profile-photo">
<img src="https://avatars.githubusercontent.com/u/127413639?s=400&u=fdfeaf957b1588b6ec9f6a862af74581873a6336&v=4" alt="Toto's Photo">
</div>
    
<h1>À propos</h1>
<p>
Je suis biostatisticien passionné par l’analyse des données. J’ai une solide expérience dans la mise en œuvre de modèles statistiques, notamment les modèles univariés, multivariés, combinatoires, ainsi que le machine learning, la détection d’anomalies, le deep learning et d’autres techniques pour l’analyse avancée des données.
</p>
<p>
En plus de ma carrière en biostatistiques, je suis passionné par la programmation web, un domaine dans lequel je m’investis activement pour créer des solutions élégantes et performantes.
</p>
<div class="tags">
<a href="https://www.w3.org/html/" target="_blank" rel="noreferrer">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/>
</a>
<a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/>
</a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/>
</a>
<a href="https://www.r-project.org/" target="_blank" rel="noreferrer">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/R_logo.svg/1200px-R_logo.svg.png" alt="r" width="40" height="40"/>
</a>
<a href="https://www.python.org" target="_blank" rel="noreferrer">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/>
</a>
<a href="https://jupyter.org/" target="_blank" rel="noreferrer">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/1200px-Jupyter_logo.svg.png" alt="jupyter" width="40" height="40"/>
</a>
</div>
</section>

<section id="experience" class="section">
<h1>Expériences</h1>
<p> Voici un aperçu de mes expériences professionnelles et académiques, incluant des projets en biostatistiques et en développement web.
</p>
</section>

<section id="projects" class="section">
<h1>Projets</h1>
<p> Cette section contiendra une liste de projets que je compléterai prochainement. Restez à l’écoute ! </p>
</section>
</div>

<script>
    const navLinks = document.querySelectorAll('.nav-link');
    const sections = document.querySelectorAll('.section');

    navLinks.forEach(link => {
      link.addEventListener('click', () => {
        // Retirer la classe active de tous les liens et sections
        navLinks.forEach(link => link.classList.remove('active'));
        sections.forEach(section => section.classList.remove('active'));

        // Ajouter la classe active au lien et à la section correspondants
        link.classList.add('active');
        const targetSection = document.getElementById(link.dataset.section);
        targetSection.classList.add('active');
      });
    });
</script>
</body>
</html>
