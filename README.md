<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Web 3D</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
        }

        #scene-container {
            width: 100vw;
            height: 100vh;
            position: absolute;
            top: 0;
            left: 0;
        }

        header {
            position: absolute;
            top: 20px;
            left: 20px;
            color: #fff;
            z-index: 1;
        }

        section {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            z-index: 1;
            color: #fff;
        }

        h1, h2 {
            color: #00A8E8;
        }

        p {
            line-height: 1.6;
        }

        footer {
            text-align: center;
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            z-index: 1;
            color: #fff;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>

    <div id="scene-container"></div>

    <header>
        <h1>Bienvenue sur ma page web 3D</h1>
    </header>

    <section>
        <h2>Introduction</h2>
        <p>Cette page web utilise des effets 3D pour une expérience interactive.</p>
        <p>Vous trouverez ci-dessous des sections pour votre CV et une présentation de votre entreprise.</p>
    </section>

    <footer>
        <p>&copy; 2024 Ma Page Web 3D</p>
    </footer>

    <script src="https://threejs.org/build/three.min.js"></script>
    <script>
        // Ajoutez ici votre code JavaScript Three.js pour les effets 3D
        // Par exemple, une sphère en rotation, un plan pour afficher le CV et la présentation de l'entreprise, etc.
    </script>

</body>
</html>
