<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="BUNKER - Jeu de société stratégique en huis clos. Plongez dans une expérience immersive de survie et de tension.">
    <meta name="keywords" content="bunker, jeu bunker, jeu de société, stratégie, survie, thinkplay">
    <title>BUNKER – Jeu de Société Stratégique</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><rect fill='%231a1a1a' width='100' height='100'/><text x='50' y='65' font-size='60' fill='%23ff4444' text-anchor='middle' font-weight='bold'>B</text></svg>">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">BUNKER</div>
            <ul class="nav-menu">
                <li><a href="#univers" onclick="navigateTo('univers')">L'Univers</a></li>
                <li><a href="#regles" onclick="navigateTo('regles')">Règles</a></li>
                <li><a href="#communaute" onclick="navigateTo('communaute')">Communauté</a></li>
                <li><a href="#acheter" onclick="navigateTo('acheter')">Acheter</a></li>
                <li class="lang-selector">
                    <select id="languageSelect" onchange="changeLanguage(this.value)">
                        <option value="fr">🇫🇷 FR</option>
                        <option value="en">🇬🇧 EN</option>
                        <option value="es">🇪🇸 ES</option>
                        <option value="it">🇮🇹 IT</option>
                    </select>
                </li>
            </ul>
            <div class="hamburger" onclick="toggleMenu()">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-overlay"></div>
        <video autoplay muted loop class="hero-video">
            <source src="data:video/mp4;base64,AAAAIGZ0eXBpc29tAAACAGlzb21pc2gtMnAw" type="video/mp4">
        </video>
        <div class="hero-content">
            <h1 class="hero-title" data-i18n="hero_title">Et si votre survie dépendait d'un jeu ?</h1>
            <p class="hero-subtitle" data-i18n="hero_subtitle">BUNKER est un jeu de société stratégique en huis clos. Incarnez des survivants après une catastrophe mondiale.</p>
            <div class="hero-ctas">
                <button class="cta-primary" onclick="navigateTo('univers')" data-i18n="btn_discover">Découvrir l'univers</button>
                <button class="cta-secondary" onclick="navigateTo('regles')" data-i18n="btn_rules">Accéder aux règles</button>
            </div>
        </div>
    </section>

    <!-- Main Content -->
    <main id="main-content">
        <!-- Accueil -->
        <section id="accueil" class="content-section active">
            <div class="section-container">
                <h2 data-i18n="welcome_title">Bienvenue dans BUNKER</h2>
                <div class="intro-card">
                    <p data-i18n="welcome_text">L'espace est limité, les ressources sont comptées, et tout le monde ne pourra pas rester. Chacun devra défendre sa place, affronter des crises collectives et convaincre les autres de sa valeur. La tension monte à chaque tour...</p>
                </div>
            </div>

            <!-- Social Wall -->
            <section class="social-wall">
                <h3 data-i18n="social_title">Suivez la communauté</h3>
                <div class="social-feed">
                    <div class="social-card">
                        <div class="social-header">
                            <span>🎮 @ThinkAndPlay</span>
                        </div>
                        <p>"Bunker lance son nouveau site ! Rejoignez la communauté 🎲"</p>
                        <a href="https://tiktok.com/@thinkplay" target="_blank">Voir sur TikTok →</a>
                    </div>
                    <div class="social-card">
                        <div class="social-header">
                            <span>📸 Instagram</span>
                        </div>
                        <p>"Une soirée Bunker intenses avec nos amis joueurs 🔥"</p>
                        <a href="https://instagram.com/thinkplay" target="_blank">Voir sur Instagram →</a>
                    </div>
                    <div class="social-card">
                        <div class="social-header">
                            <span>💼 LinkedIn</span>
                        </div>
                        <p>"Bunker : quand le jeu de société rencontre la stratégie..."</p>
                        <a href="https://linkedin.com/company/thinkplay" target="_blank">Voir sur LinkedIn →</a>
                    </div>
                </div>
            </section>
        </section>

        <!-- Univers -->
        <section id="univers" class="content-section">
            <div class="section-container">
                <h2 data-i18n="univers_title">L'Univers de BUNKER</h2>
                
                <div class="univers-intro">
                    <p data-i18n="univers_intro">Après une catastrophe mondiale, l'humanité s'est réfugiée sous terre. Dans ce bunker souterrain, les survivants font face à des dilemmes impossibles : qui mérite de rester ? Qui est une menace ? Chaque décision peut changer le cours de la partie.</p>
                </div>

                <div class="characters-grid">
                    <div class="character-card">
                        <div class="character-icon">🔬</div>
                        <h4 data-i18n="char_scientist">La Scientifique</h4>
                        <p data-i18n="char_scientist_desc">Elle connaît les secrets du bunker et les ressources disponibles. Mais peut-on lui faire confiance ?</p>
                    </div>
                    <div class="character-card">
                        <div class="character-icon">🎖️</div>
                        <h4 data-i18n="char_military">Le Militaire</h4>
                        <p data-i18n="char_military_desc">Habitué aux crises, il cherche à maintenir l'ordre. Ou à prendre le contrôle ?</p>
                    </div>
                    <div class="character-card">
                        <div class="character-icon">📚</div>
                        <h4 data-i18n="char_teacher">L'Enseignante</h4>
                        <p data-i18n="char_teacher_desc">Elle croit en la coopération et l'humanité. Mais naïveté et altruisme peuvent être des faiblesses.</p>
                    </div>
                    <div class="character-card">
                        <div class="character-icon">🕵️</div>
                        <h4 data-i18n="char_suspect">L'Énigmatique</h4>
                        <p data-i18n="char_suspect_desc">Qui est-il vraiment ? Pourquoi garde-t-il ses secrets ? Peut-être la clé de la survie.</p>
                    </div>
                </div>

                <div class="univers-teasing">
                    <p data-i18n="univers_teasing">Mais pour connaître l'issue de cette lutte pour la survie, vous devrez vous aussi franchir la porte du Bunker...</p>
                    <button class="cta-primary" onclick="navigateTo('acheter')" data-i18n="btn_buy">Acheter le jeu</button>
                </div>
            </div>
        </section>

        <!-- Règles -->
        <section id="regles" class="content-section">
            <div class="section-container">
                <h2 data-i18n="regles_title">Règles du Jeu</h2>
                
                <div class="rules-tabs">
                    <button class="tab-btn active" onclick="switchTab(event, 'setup')" data-i18n="tab_setup">Mise en place</button>
                    <button class="tab-btn" onclick="switchTab(event, 'gameplay')" data-i18n="tab_gameplay">Déroulement</button>
                    <button class="tab-btn" onclick="switchTab(event, 'crisis')" data-i18n="tab_crisis">Crises</button>
                    <button class="tab-btn" onclick="switchTab(event, 'victory')" data-i18n="tab_victory">Victoire</button>
                    <button class="tab-btn" onclick="switchTab(event, 'lexique')" data-i18n="tab_lexique">Lexique</button>
                </div>

                <!-- Setup Tab -->
                <div id="setup" class="tab-content active">
                    <h3 data-i18n="setup_title">Mise en place</h3>
                    <ol>
                        <li><strong data-i18n="setup_1_title">Joueurs :</strong> <span data-i18n="setup_1_desc">2 à 6 joueurs (optimal : 4-5)</span></li>
                        <li><strong data-i18n="setup_2_title">Durée :</strong> <span data-i18n="setup_2_desc">45 à 90 minutes selon le nombre de joueurs</span></li>
                        <li><strong data-i18n="setup_3_title">Distribution :</strong> <span data-i18n="setup_3_desc">Chaque joueur reçoit une fiche rôle et des cartes ressources initiales</span></li>
                        <li><strong data-i18n="setup_4_title">Ressources :</strong> <span data-i18n="setup_4_desc">Placez les jetons ressources au centre de la table</span></li>
                        <li><strong data-i18n="setup_5_title">Premier joueur :</strong> <span data-i18n="setup_5_desc">Le joueur le plus jeune commence</span></li>
                    </ol>
                </div>

                <!-- Gameplay Tab -->
                <div id="gameplay" class="tab-content">
                    <h3 data-i18n="gameplay_title">Déroulement d'une partie</h3>
                    <div class="rule-block">
                        <h4 data-i18n="round_title">Chaque tour :</h4>
                        <ol>
                            <li data-i18n="round_1">Un joueur active une action (commerce, négociation, sabotage)</li>
                            <li data-i18n="round_2">Les autres joueurs peuvent réagir ou contester cette action</li>
                            <li data-i18n="round_3">Les ressources se gèrent selon les règles en vigueur</li>
                            <li data-i18n="round_4">Un nouveau tour commence avec le joueur suivant</li>
                        </ol>
                    </div>
                </div>

                <!-- Crisis Tab -->
                <div id="crisis" class="tab-content">
                    <h3 data-i18n="crisis_title">Les Crises</h3>
                    <p data-i18n="crisis_intro">À chaque tour impair, une crise se déclenche. Les joueurs doivent ensemble trouver une solution.</p>
                    <ul>
                        <li><strong data-i18n="crisis_1_title">Pénurie d'eau :</strong> <span data-i18n="crisis_1_desc">Tout le monde perd 2 ressources eau</span></li>
                        <li><strong data-i18n="crisis_2_title">Révolte :</strong> <span data-i18n="crisis_2_desc">Les joueurs votent pour éliminer un survivant</span></li>
                        <li><strong data-i18n="crisis_3_title">Défaillance système :</strong> <span data-i18n="crisis_3_desc">Une partie du bunker devient inaccessible</span></li>
                    </ul>
                </div>

                <!-- Victory Tab -->
                <div id="victory" class="tab-content">
                    <h3 data-i18n="victory_title">Conditions de Victoire</h3>
                    <p data-i18n="victory_coop">Le jeu offre plusieurs modes de victoire :</p>
                    <ul>
                        <li><strong data-i18n="victory_1">Mode Coopératif :</strong> <span data-i18n="victory_1_desc">Tous les survivants émergent ensemble après 10 tours</span></li>
                        <li><strong data-i18n="victory_2">Mode Compétitif :</strong> <span data-i18n="victory_2_desc">Le dernier survivant debout gagne</span></li>
                        <li><strong data-i18n="victory_3">Mode Équilibré :</strong> <span data-i18n="victory_3_desc">Comptez les points à la fin (ressources + influence)</span></li>
                    </ul>
                </div>

                <!-- Lexique Tab -->
                <div id="lexique" class="tab-content">
                    <h3 data-i18n="lexique_title">Lexique</h3>
                    <div class="lexique-grid">
                        <div class="lexique-item">
                            <strong data-i18n="lex_ressource">Ressource</strong>
                            <p data-i18n="lex_ressource_def">Eau, nourriture, énergie. Essentielles pour survivre.</p>
                        </div>
                        <div class="lexique-item">
                            <strong data-i18n="lex_vote">Vote</strong>
                            <p data-i18n="lex_vote_def">Les joueurs décident collectivement d'une action.</p>
                        </div>
                        <div class="lexique-item">
                            <strong data-i18n="lex_sabotage">Sabotage</strong>
                            <p data-i18n="lex_sabotage_def">Bloquer secrètement une action d'un autre joueur.</p>
                        </div>
                        <div class="lexique-item">
                            <strong data-i18n="lex_crise">Crise</strong>
                            <p data-i18n="lex_crise_def">Événement menaçant nécessitant une action collective.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Communauté -->
        <section id="communaute" class="content-section">
            <div class="section-container">
                <h2 data-i18n="community_title">Communauté BUNKER</h2>
                
                <div class="community-intro">
                    <p data-i18n="community_desc">Rejoignez des milliers de joueurs passionnés. Organisez des parties, partagez vos stratégies et votre expérience.</p>
                </div>

                <div class="community-sections">
                    <div class="community-card">
                        <h3 data-i18n="events_title">🎮 Événements</h3>
                        <p data-i18n="events_desc">Découvrez les soirées Bunker organisées près de vous.</p>
                        <div class="event-list">
                            <div class="event-item">
                                <strong data-i18n="event_1_title">Festival Ludique - Nantes</strong>
                                <p data-i18n="event_1_date">15 Mars 2026 - Salle municipale</p>
                            </div>
                            <div class="event-item">
                                <strong data-i18n="event_2_title">Tournoi Compétitif - Paris</strong>
                                <p data-i18n="event_2_date">22 Avril 2026 - Café des jeux</p>
                            </div>
                        </div>
                    </div>

                    <div class="community-card">
                        <h3 data-i18n="forum_title">💬 Forum</h3>
                        <p data-i18n="forum_desc">Posez vos questions, partagez vos variantes de règles.</p>
                        <ul>
                            <li><a href="#" data-i18n="forum_1">Stratégies gagnantes</a></li>
                            <li><a href="#" data-i18n="forum_2">Variantes maison</a></li>
                            <li><a href="#" data-i18n="forum_3">Questions sur les règles</a></li>
                        </ul>
                    </div>

                    <div class="community-card">
                        <h3 data-i18n="social_community_title">📱 Réseaux</h3>
                        <p data-i18n="social_community_desc">Suivez l'actualité Bunker en direct.</p>
                        <div class="social-links">
                            <a href="https://tiktok.com/@thinkplay" target="_blank">TikTok 🎬</a>
                            <a href="https://instagram.com/thinkplay" target="_blank">Instagram 📸</a>
                            <a href="https://linkedin.com/company/thinkplay" target="_blank">LinkedIn 💼</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Acheter -->
        <section id="acheter" class="content-section">
            <div class="section-container buy-section">
                <h2 data-i18n="buy_title">Prêt à entrer dans le BUNKER ?</h2>
                
                <div class="buy-card">
                    <h3 data-i18n="buy_cta">Le jeu est disponible ici :</h3>
                    
                    <div class="buy-info">
                        <div class="info-item">
                            <strong data-i18n="buy_price">Prix indicatif :</strong>
                            <span>29,99 €</span>
                        </div>
                        <div class="info-item">
                            <strong data-i18n="buy_box">Contenu de la boîte :</strong>
                            <ul>
                                <li data-i18n="buy_box_1">1 plateau de jeu</li>
                                <li data-i18n="buy_box_2">60 cartes</li>
                                <li data-i18n="buy_box_3">100 jetons ressources</li>
                                <li data-i18n="buy_box_4">1 livret de règles complet</li>
                                <li data-i18n="buy_box_5">Feuilles de score</li>
                            </ul>
                        </div>
                    </div>

                    <a href="https://www.thinkplay.fr/" target="_blank" class="cta-massive" data-i18n="btn_buy_massive">ACHETER LE JEU SUR THINKPLAY.FR</a>

                    <div class="buy-guarantee">
                        <p data-i18n="buy_guarantee">✓ Livraison rapide | ✓ Garantie 2 ans | ✓ Support client 24/7</p>
                    </div>

                    <div class="buy-professional">
                        <h4 data-i18n="buy_pro_title">Vous êtes distributeur ou revendeur ?</h4>
                        <p data-i18n="buy_pro_desc">Contactez-nous pour des conditions commerciales spéciales.</p>
                        <a href="mailto:contact@thinkplay.fr" class="email-link">contact@thinkplay.fr</a>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-content">
            <div class="footer-section">
                <h4>BUNKER</h4>
                <p data-i18n="footer_tagline">Un jeu de société immersif par Think&Play</p>
            </div>
            <div class="footer-section">
                <h4 data-i18n="footer_links">Liens</h4>
                <ul>
                    <li><a href="https://www.thinkplay.fr/" target="_blank" data-i18n="footer_thinkplay">Think&Play</a></li>
                    <li><a href="https://trictrac.net" target="_blank" data-i18n="footer_trictrac">Tric Trac</a></li>
                    <li><a href="https://boardgamegeek.com" target="_blank" data-i18n="footer_bgg">BoardGameGeek</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h4 data-i18n="footer_contact">Contact</h4>
                <p><a href="mailto:contact@thinkplay.fr">contact@thinkplay.fr</a></p>
                <p>+33 (0) 2 XX XX XX XX</p>
            </div>
        </div>
        <div class="footer-bottom">
            <p data-i18n="footer_copy">&copy; 2026 Think&Play. Tous droits réservés.</p>
        </div>
    </footer>

    <script src="js/script.js"></script>
</body>
</html>
