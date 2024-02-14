<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mon Entreprise - À Propos de Moi</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            overflow: hidden;
            background-color: #001F3F; /* Fond bleu marine */
            color: #fff;
        }

        header {
            background-color: #0C1821; /* Bleu marine plus foncé pour l'en-tête */
            padding: 20px;
            text-align: center;
            color: #fff;
        }

        nav {
            background-color: #001F3F;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            padding: 15px;
            margin: 0 10px;
            font-weight: bold;
            cursor: pointer;
        }

        section {
            padding: 20px;
            position: relative;
            display: none;
        }

        #entreprise {
            display: block;
        }

        #apropos {
            display: none;
        }

        .justifier {
            text-align: justify;
        }

        h1, h2 {
            color: #0C1821;
        }

        p {
            line-height: 1.6;
        }

        footer {
            background-color: #001F3F;
            color: #fff;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        /* Styles pour les étoiles animées en arrière-plan */
        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }

        .star {
            position: absolute;
            background-color: #fff;
            border-radius: 50%;
            animation: twinkle 1s infinite;
        }

        @keyframes twinkle {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
                opacity: 0.8;
            }
        }
    </style>
</head>
<body>

    <!-- Étoiles animées en arrière-plan -->
    <div class="stars">
        <!-- Vous pouvez ajuster le nombre d'étoiles en dupliquant ces divs -->
        <div class="star" style="top: 10%; left: 25%; width: 2px; height: 2px;"></div>
        <div class="star" style="top: 50%; left: 70%; width: 2px; height: 2px;"></div>
        <!-- ... Ajoutez plus d'étoiles selon vos préférences ... -->
    </div>

    <header>
        <h1>Mon Entreprise</h1>
        <p>Vente de prestations de développement informatique</p>
    </header>

    <nav>
        <a onclick="showTab('entreprise')">Entreprise</a>
        <a onclick="showTab('apropos')">À Propos de Moi</a>
    </nav>

    <section id="entreprise" class="justifier">
        <h2>À Propos de Mon Entreprise</h2>
        <p>
            En tant qu'auto-entrepreneur passionné par le développement informatique, je propose des prestations sur mesure pour répondre aux besoins variés de mes clients.
            Mon objectif est de fournir des solutions de qualité et innovantes, en mettant en avant mes compétences techniques et mon engagement envers l'excellence.
        </p>
        <p>Explorez nos services et découvrez comment nous pouvons vous aider à atteindre vos objectifs numériques.</p>
    </section>

    <section id="apropos">
        <h2>À Propos de Moi</h2>
        <p>
            En tant qu'étudiant passionné par le monde de l'informatique, j'ai créé mon entreprise pour offrir des services de développement informatique et de création de logiciels sur mesure.
            Mon objectif est de mettre mes compétences techniques au service de ceux qui recherchent des solutions numériques adaptées à leurs besoins spécifiques. Une entreprise dédiée à fournir des solutions innovantes et de qualité.
        </p>
        <p>Consultez mon CV pour en savoir plus sur mon parcours professionnel et mes compétences.</p>
        <!-- Ajoutez ici un lien vers votre CV ou intégrez-le directement -->
    </section>

    <footer>
        <p>&copy; 2024 Mon Entreprise - À Propos de Moi</p>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <script>
        function showTab(tabName) {
            document.getElementById('entreprise').style.display = (tabName === 'entreprise') ? 'block' : 'none';
            document.getElementById('apropos').style.display = (tabName === 'apropos') ? 'block' : 'none';
        }
    </script>
</body>
</html>
