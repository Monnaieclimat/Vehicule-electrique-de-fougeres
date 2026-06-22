# Vehicule-electrique-de-fougeres
Ventes de véhicules electrique à fougeres
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Les Voitures Électriques de Fougères</title>
    <style>
        :root {
            --edf-blue: #0066CC; /* Bleu EDF */
            --byd-red: #D52B1E; /* Rouge BYD */
            --renault-yellow: #FFC700; /* Jaune Renault */
            --tesla-red: #E31E24; /* Rouge Tesla */
            --neutral-gray: #F5F5F5; /* Gris clair */
            --dark-gray: #333333; /* Gris foncé */
            --white: #FFFFFF;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--edf-blue); /* Fond bleu EDF */
            color: var(--dark-gray);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1621799754526-a0d52c49fad5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            color: var(--white);
            padding: 80px 0;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .logo {
            font-size: 32px;
            font-weight: bold;
            color: var(--white);
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
        }

        .tagline {
            font-size: 18px;
            opacity: 0.9;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.8);
        }

        nav {
            background-color: var(--white);
            padding: 15px 0;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav .nav-container {
            display: flex;
            justify-content: space-around;
            max-width: 1200px;
            margin: 0 auto;
        }

        nav a {
            color: var(--dark-gray);
            text-decoration: none;
            font-weight: 600;
            padding: 10px 20px;
            border-radius: 5px;
            transition: all 0.3s;
        }

        nav a:hover {
            background-color: var(--edf-blue);
            color: var(--white);
        }

        .hero {
            text-align: center;
            padding: 40px 20px;
        }

        .hero h1 {
            font-size: 48px;
            color: var(--white);
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
        }

        .hero p {
            font-size: 20px;
            max-width: 800px;
            margin: 0 auto 30px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.8);
        }

        .btn {
            display: inline-block;
            background-color: var(--edf-blue);
            color: var(--white);
            padding: 12px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background-color: #0052A3;
        }

        .brands-section {
            padding: 60px 0;
            text-align: center;
            background-color: var(--white);
        }

        .brands-section h2 {
            color: var(--edf-blue);
            font-size: 36px;
            margin-bottom: 40px;
        }

        .brands-grid {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 30px;
        }

        .brand-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 20px;
            width: 300px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .brand-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .brand-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .brand-card .brand-logo {
            height: 40px;
            margin-bottom: 15px;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .brand-card h3 {
            color: var(--dark-gray);
            margin-bottom: 10px;
            font-size: 20px;
        }

        .brand-card p {
            color: var(--dark-gray);
            margin-bottom: 20px;
            font-size: 14px;
        }

        .brand-card .brand-btn {
            background-color: var(--edf-blue);
        }

        .byd .brand-btn {
            background-color: var(--byd-red);
        }

        .renault .brand-btn {
            background-color: var(--renault-yellow);
            color: var(--dark-gray);
        }

        .tesla .brand-btn {
            background-color: var(--tesla-red);
        }

        .advantages-section {
            background-color: var(--white);
            padding: 60px 0;
        }

        .advantages-section h2 {
            text-align: center;
            color: var(--edf-blue);
            font-size: 36px;
            margin-bottom: 40px;
        }

        .advantages-grid {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 30px;
        }

        .advantage-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 30px;
            width: 300px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s;
            border: 1px solid #e0e0e0;
        }

        .advantage-card:hover {
            transform: translateY(-10px);
        }

        .advantage-card .icon {
            font-size: 50px;
            margin-bottom: 15px;
        }

        .advantage-card h3 {
            color: var(--edf-blue);
            margin-bottom: 15px;
        }

        .stats-section {
            padding: 40px 0;
            text-align: center;
            background-color: var(--white);
        }

        .stats-grid {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
        }

        .stat-item {
            background-color: var(--white);
            border-radius: 10px;
            padding: 20px;
            width: 200px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border: 1px solid #e0e0e0;
        }

        .stat-item h4 {
            color: var(--edf-blue);
            margin-bottom: 10px;
        }

        .stat-item p {
            font-size: 24px;
            font-weight: bold;
            color: var(--dark-gray);
            margin: 0;
        }

        .stat-item .subtext {
            font-size: 14px;
            color: #666666;
            margin-top: 5px;
        }

        footer {
            background-color: var(--dark-gray);
            color: var(--white);
            text-align: center;
            padding: 30px 0;
            margin-top: 50px;
        }

        @media (max-width: 768px) {
            .brands-grid, .advantages-grid, .stats-grid {
                flex-direction: column;
                align-items: center;
            }
            nav .nav-container {
                flex-direction: column;
                gap: 10px;
            }
            .hero h1 {
                font-size: 36px;
            }
            header {
                padding: 60px 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">Les Voitures Électriques de Fougères</div>
            <p class="tagline">Votre partenaire pour la mobilité électrique en Bretagne</p>
            <div class="hero">
                <h1>Découvrez l'avenir de la mobilité</h1>
                <p>Explorez notre sélection de véhicules 100% électriques, alliant performance, écologie et économie. Roulez propre, roulez intelligent !</p>
                <a href="#marques" class="btn">Voir nos marques</a>
            </div>
        </div>
    </header>

    <nav>
        <div class="nav-container">
            <a href="#accueil">Accueil</a>
            <a href="#marques">Nos Marques</a>
            <a href="#avantages">Avantages</a>
            <a href="#catalogue">Catalogue</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <section id="marques" class="brands-section">
        <div class="container">
            <h2>Nos Marques Principales</h2>
            <div class="brands-grid">
                <div class="brand-card byd">
                    <img src="images/byd-seal-gt07.jpg" alt="BYD Seal GT 07">
                    <div class="brand-logo">
                        <svg width="80" height="30" viewBox="0 0 80 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect width="80" height="30" fill="#D52B1E"/>
                            <text x="40" y="20" font-family="Arial, sans-serif" font-size="14" fill="white" text-anchor="middle" font-weight="bold">BYD</text>
                        </svg>
                    </div>
                    <h3>BYD</h3>
                    <p>Innovation chinoise, leader mondial des véhicules électriques. Des modèles accessibles et performants comme le <strong>Seal GT 07</strong>.</p>
                    <a href="#catalogue" class="btn brand-btn">Voir les modèles BYD</a>
                </div>
                <div class="brand-card renault">
                    <img src="images/renault-r5.jpg" alt="Renault R5">
                    <div class="brand-logo">
                        <svg width="100" height="30" viewBox="0 0 100 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect width="100" height="30" fill="#FFC700"/>
                            <text x="50" y="20" font-family="Arial, sans-serif" font-size="12" fill="#333333" text-anchor="middle" font-weight="bold">RENAULT</text>
                        </svg>
                    </div>
                    <h3>Renault</h3>
                    <p>Expertise française, avec des modèles emblématiques comme la <strong>R5</strong>, alliant design rétro et technologie moderne.</p>
                    <a href="#catalogue" class="btn brand-btn">Voir les modèles Renault</a>
                </div>
                <div class="brand-card tesla">
                    <img src="images/tesla-model3.jpg" alt="Tesla Model 3">
                    <div class="brand-logo">
                        <svg width="80" height="30" viewBox="0 0 80 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect width="80" height="30" fill="#E31E24"/>
                            <text x="40" y="20" font-family="Arial, sans-serif" font-size="14" fill="white" text-anchor="middle" font-weight="bold">TESLA</text>
                        </svg>
                    </div>
                    <h3>Tesla</h3>
                    <p>Technologie de pointe, autonomie exceptionnelle et accélération impressionnante avec la <strong>Model 3</strong>.</p>
                    <a href="#catalogue" class="btn brand-btn">Voir les modèles Tesla</a>
                </div>
            </div>
        </div>
    </section>

    <section id="avantages" class="advantages-section">
        <div class="container">
            <h2>Pourquoi choisir l'électrique ?</h2>
            <div class="advantages-grid">
                <div class="advantage-card">
                    <div class="icon">💰</div>
                    <h3>Coût au km réduit</h3>
                    <p>Économisez jusqu'à <strong>70%</strong> sur le coût au kilomètre par rapport à un véhicule thermique. Avec l'électricité, finies les fluctuations du prix du carburant !</p>
                    <p><strong>Exemple :</strong> 2€/100km contre 8€/100km pour une voiture essence.</p>
                </div>
                <div class="advantage-card">
                    <div class="icon">🔧</div>
                    <h3>Entretien simplifié</h3>
                    <p>Moins de pièces d'usure : pas de vidange, pas de courroie de distribution, pas d'embrayage. Un entretien réduit de <strong>30 à 50%</strong>.</p>
                    <p><strong>Économies annuelles :</strong> Jusqu'à 500€/an en moins par rapport à un véhicule thermique.</p>
                </div>
                <div class="advantage-card">
                    <div class="icon">🌱</div>
                    <h3>Bilan carbone optimisé</h3>
                    <p>Zéro émission locale et jusqu'à <strong>90% de CO₂ en moins</strong> sur l'ensemble du cycle de vie (même en incluant la production de la batterie).</p>
                    <p><strong>Impact :</strong> 2 tonnes de CO₂ évitées par an pour 15 000 km parcourus.</p>
                </div>
            </div>

            <div class="stats-section">
                <div class="stats-grid">
                    <div class="stat-item">
                        <h4>Économies annuelles</h4>
                        <p>1 200€</p>
                        <p class="subtext">par an vs thermique</p>
                    </div>
                    <div class="stat-item">
                        <h4>CO₂ évité</h4>
                        <p>2 tonnes</p>
                        <p class="subtext">par an et par voiture</p>
                    </div>
                    <div class="stat-item">
                        <h4>Autonomie moyenne</h4>
                        <p>400 km</p>
                        <p class="subtext">par charge</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="catalogue" class="container" style="padding: 60px 0; text-align: center; background-color: var(--white);">
        <h2 style="color: var(--edf-blue); font-size: 36px; margin-bottom: 20px;">Catalogue des véhicules</h2>
        <p style="max-width: 800px; margin: 0 auto 30px;">Découvrez tous nos modèles disponibles chez <strong>Les Voitures Électriques de Fougères</strong>.</p>
        <a href="#" class="btn">Voir le catalogue complet</a>
    </section>

    <section id="contact" class="container" style="padding: 60px 0; text-align: center; background-color: var(--white);">
        <h2 style="color: var(--edf-blue); font-size: 36px; margin-bottom: 20px;">Contactez-nous</h2>
        <p style="max-width: 800px; margin: 0 auto 30px;">Prêt à passer à l'électrique ? Contactez-nous pour un essai ou pour plus d'informations. Nous sommes basés à Fougères, en Bretagne.</p>
        <a href="mailto:contact@voitures-electriques-fougeres.fr" class="btn">Nous contacter</a>
        <p style="margin-top: 30px; font-size: 18px;">
            📍 1 Rue de la Forêt, 35133 Fougères<br>
            ☎️ 02 99 99 99 99
        </p>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2026 Les Voitures Électriques de Fougères. Tous droits réservés.</p>
            <p style="margin-top: 10px;">Roulez propre, roulez breton !</p>
        </div>
    </footer>
</body>
</html>
