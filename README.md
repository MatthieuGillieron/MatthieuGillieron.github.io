<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CV - Matthieu Gillieron</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            font-size: 11px;
            line-height: 1.4;
            color: #2d3748;
            background: #f7fafc;
        }
        
        @media print {
            * {
                -webkit-print-color-adjust: exact !important;
                color-adjust: exact !important;
            }
            body { 
                font-size: 10px; 
                background: white;
            }
            .container { 
                margin: 0; 
                box-shadow: none; 
            }
        }
        
        .container {
            max-width: 210mm;
            height: auto;
            min-height: 297mm;
            margin: 20px auto;
            display: grid;
            grid-template-columns: 280px 1fr;
            background: white;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
            border-radius: 8px;
            overflow: visible;
        }
        
        .sidebar {
            background: linear-gradient(135deg, #718096 0%, #4a5568 100%);
            color: white;
            padding: 30px 25px 30px 25px;
        }
        
        .profile-section {
            text-align: center;
            margin-bottom: 25px;
        }
        
        .profile-photo {
            width: 135px;
            height: 135px;
            border-radius: 50%;
            background-image: url('image/4.png');
            background-size: cover;
            background-position: center;
            margin: 0 auto 20px;
        }
        
        .main {
            padding: 30px 30px 25px 30px;
            background: white;
        }
        
        .main section {
            margin-bottom: 20px;
        }
        
        .name {
            font-size: 20px;
            font-weight: 700;
            text-align: center;
            margin-bottom: 8px;
            letter-spacing: 0.5px;
        }
        
        .title {
            font-size: 14px;
            text-align: center;
            margin-bottom: 20px;
            font-weight: 400;
            color: rgba(255,255,255,0.9);
        }
        
        .separator {
            width: 100%;
            height: 1px;
            background: rgba(255,255,255,0.3);
            margin-bottom: 30px;
        }
        
        .section-separator {
            width: 100%;
            height: 1px;
            background: rgba(255,255,255,0.3);
            margin: 20px 0;
        }
        
        .sidebar .section-title {
            color: white;
            font-size: 12px;
            font-weight: 600;
            text-transform: uppercase;
            margin-bottom: 15px;
            letter-spacing: 0.5px;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .main .section-title {
            color: #4a5568;
            font-size: 15px;
            font-weight: 600;
            text-transform: uppercase;
            border-bottom: 2px solid #e2e8f0;
            margin-bottom: 15px;
            padding-bottom: 8px;
            letter-spacing: 0.5px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 12px;
            font-size: 10px;
            line-height: 1.4;
        }
        
        .contact-item i {
            width: 20px;
            margin-right: 12px;
            font-size: 11px;
            color: rgba(255,255,255,0.9);
            text-align: center;
        }
        
        .skill-group {
            margin-bottom: 15px;
        }
        
        .skill-group h4 {
            font-size: 11px;
            font-weight: 600;
            margin-bottom: 8px;
            color: rgba(255,255,255,0.95);
            text-transform: uppercase;
            letter-spacing: 0.3px;
            display: flex;
            align-items: center;
            gap: 6px;
        }
        
        .skill-item {
            display: inline-block;
            background: rgba(255,255,255,0.15);
            padding: 4px 8px;
            margin: 2px 3px;
            border-radius: 12px;
            font-size: 8px;
            font-weight: 500;
            border: 1px solid rgba(255,255,255,0.2);
        }
        
        .experience-item {
            margin-bottom: 18px;
            padding-bottom: 15px;
            border-bottom: 1px solid #e2e8f0;
        }
        
        .experience-item:last-child {
            border-bottom: none;
            margin-bottom: 0;
        }
        
        .exp-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 8px;
        }
        
        .exp-title {
            font-size: 14px;
            font-weight: 600;
            color: #4a5568;
            margin-bottom: 3px;
        }
        
        .exp-company {
            font-size: 12px;
            color: #718096;
            font-weight: 500;
        }
        
        .exp-date {
            font-size: 10px;
            color: #a0aec0;
            white-space: nowrap;
            font-weight: 500;
        }
        
        .exp-desc {
            font-size: 11px;
            line-height: 1.5;
        }
        
        .exp-desc li {
            margin-bottom: 4px;
            list-style: none;
            padding-left: 15px;
            position: relative;
        }
        
        .exp-desc li::before {
            content: "▸";
            position: absolute;
            left: 0;
            color: #718096;
            font-weight: bold;
        }
        
        .profile {
            font-size: 12px;
            line-height: 1.6;
            margin-bottom: 15px;
            text-align: justify;
            color: #4a5568;
        }
        
        .highlight {
            color: #4a5568;
            font-weight: 600;
        }
        
        .soft-skills {
            font-size: 9px;
            line-height: 1.5;
        }
        
        .soft-skills li {
            margin-bottom: 8px;
            list-style: none;
            padding-left: 15px;
            position: relative;
            color: rgba(255,255,255,0.9);
        }
        
        .soft-skills li::before {
            content: "▸";
            position: absolute;
            left: 0;
            color: rgba(255,255,255,0.7);
            font-weight: bold;
        }
        
        .languages {
            font-size: 10px;
        }
        
        .language-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
            color: rgba(255,255,255,0.9);
        }
        
        .language-level {
            font-weight: 500;
            color: rgba(255,255,255,0.7);
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Sidebar -->
        <div class="sidebar">
            <div class="profile-section">
                <div class="profile-photo"></div>
                <h1 class="name">MATTHIEU GILLIERON</h1>
                <p class="title">Junior AI Engineer</p>
                <div class="separator"></div>
            </div>
            
            <!-- Infos -->
            <div class="section" style="margin-bottom: 25px;">
                <h2 class="section-title">
                    <i class="fas fa-address-card"></i>
                    Infos
                </h2>
                <div class="contact-item">
                    <i class="fas fa-phone"></i>
                    <span>079 921 81 40</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <span>gillieron.matthieu@gmail.com</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <span>Route de Champery 4, 1873 Val-D'Illiez, Suisse</span>
                </div>
                <div class="contact-item">
                    <i class="fab fa-linkedin"></i>
                    <span>linkedin.com/in/matthieu-gillieron-developer</span>
                </div>
                <div class="contact-item">
                    <i class="fab fa-github"></i>
                    <span>github.com/MatthieuGillieron</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-birthday-cake"></i>
                    <span>23 ans</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-car"></i>
                    <span>Permis A1, B, C, BE, CE</span>
                </div>
            </div>
            
            <div class="section-separator"></div>
            
            <div class="section" style="margin-bottom: 20px;">
                <div class="skill-group">
                    <h4><i class="fas fa-laptop-code"></i> Langages</h4>
                    <div class="skill-list">
                        <span class="skill-item" style="font-weight: bold;">Python</span>
                        <span class="skill-item">C</span>
                        <span class="skill-item">C++</span>
                        <span class="skill-item">JavaScript</span>
                    </div>
                </div>
                
                <div class="skill-group">
                    <h4><i class="fas fa-tools"></i> Frameworks</h4>
                    <div class="skill-list">
                        <span class="skill-item" style="font-weight: bold;">FastAPI</span>
                        <span class="skill-item" style="font-weight: bold;">Streamlit</span>
                        <span class="skill-item">React</span>
                        <span class="skill-item">LangChain</span>
                    </div>
                </div>
                
                <div class="skill-group">
                    <h4><i class="fas fa-brain"></i> Intelligence Artificielle</h4>
                    <div class="skill-list">
                        <span class="skill-item" style="font-weight: bold;">RAG</span>
                        <span class="skill-item" style="font-weight: bold;">ChromaDB</span>
                        <span class="skill-item" style="font-weight: bold;">Vector DB</span>
                        <span class="skill-item" style="font-weight: bold;">OpenAI API</span>
                        <span class="skill-item" style="font-weight: bold;">Claude API</span>
                        <span class="skill-item">NLP</span>
                    </div>
                </div>
                
                <div class="skill-group">
                    <h4><i class="fas fa-database"></i> Technologies</h4>
                    <div class="skill-list">
                        <span class="skill-item">PostgreSQL</span>
                        <span class="skill-item">Docker</span>
                        <span class="skill-item">Git/GitHub</span>
                    </div>
                </div>
            </div>
            
            <div class="section-separator"></div>
            
            <!-- Soft Skills -->
            <div class="section" style="margin-bottom: 25px;">
                <h2 class="section-title">
                    <i class="fas fa-lightbulb"></i>
                    Soft Skills
                </h2>
                <ul class="soft-skills">
                    <li>Adaptabilité et apprentissage continu</li>
                    <li>Communication efficace et esprit d'équipe</li>
                    <li>Curiosité et détermination</li>
                    <li>Rigueur et approche pragmatique</li>
                    <li>Résolution créative de problèmes</li>
                </ul>
            </div>
            
            <div class="section-separator"></div>
            
            <!-- Langues -->
            <div class="section">
                <h2 class="section-title">
                    <i class="fas fa-globe"></i>
                    Langues
                </h2>
                <div class="languages">
                    <div class="language-item">
                        <span>Français</span>
                        <span class="language-level">Natif</span>
                    </div>
                    <div class="language-item">
                        <span>Anglais</span>
                        <span class="language-level">Intermédiaire</span>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Main Content -->
        <div class="main">
            <!-- Profil -->
            <section>
                <h2 class="section-title">
                    <i class="fas fa-user-circle"></i>
                    Résumé
                </h2>
                <p class="profile">
                    <span class="highlight">Junior AI Engineer</span> passionné par l'intelligence artificielle et le développement web. Jeune professionnel <span class="highlight">curieux et déterminé</span>, toujours en quête d'apprentissage et de dépassement de soi. Expérience pratique en <span class="highlight">RAG multimodal</span>, chatbots IA et développement full-stack.
                </p>
            </section>
            
            <!-- Projets Techniques -->
            <section>
                <h2 class="section-title">
                    <i class="fas fa-project-diagram"></i>
                    Projets Techniques
                </h2>
                
                <div class="experience-item">
                    <div class="exp-header">
                        <div>
                            <div class="exp-title">Chatbot RAG Multimodal</div>
                            <div class="exp-company">Projet Personnel - Intelligence Artificielle</div>
                        </div>
                        <div class="exp-date">2025</div>
                    </div>
                    <ul class="exp-desc">
                        <li>Création d'un <span class="highlight">chatbot RAG multimodal</span> pour l'apprentissage des technologies IA</li>
                        <li>Intégration de <span class="highlight">vector databases</span> et traitement de données multimodales</li>
                        <li>Tech : Python, <span class="highlight">LangChain</span>, ChromaDB, OpenAI API</li>
                    </ul>
                </div>
                
                <div class="experience-item">
                    <div class="exp-header">
                        <div>
                            <div class="exp-title">Hackathon IA Innovation Lab</div>
                            <div class="exp-company">Chatbot d'Orientation IT - <span class="highlight">Équipe Gagnante</span></div>
                        </div>
                        <div class="exp-date">2025</div>
                    </div>
                    <ul class="exp-desc">
                        <li><span class="highlight">Chatbot RAG</span> + Partie pratique pour orienter les jeunes vers les métiers IT</li>
                        <li>Entraîné sur données d'écoles et emplois suisses</li>
                        <li>Partie pratique de 4 métiers : dev. frontend, backend, cybersécurité, gamedev</li>
                        <li>Tech : Python, <span class="highlight">Streamlit</span>, RAG, <span class="highlight">ChromaDB</span></li>
                    </ul>
                </div>
                
                <div class="experience-item">
                    <div class="exp-header">
                        <div>
                            <div class="exp-title">Hackathon Infomiak</div>
                            <div class="exp-company">Intégration IA - <span class="highlight">Équipe Gagnante</span></div>
                        </div>
                        <div class="exp-date">2025</div>
                    </div>
                    <ul class="exp-desc">
                        <li><span class="highlight">Victoire</span> avec équipe aléatoire sur l'intégration IA dans système de mails</li>
                        <li>Développement de solutions <span class="highlight">NLP</span> pour automatisation email</li>
                        <li>Injection de la solution via <span class="highlight">extension Chrome</span> dans leur système (kSuite) pour intégrer le frontend</li>
                        <li>Collaboration efficace et résolution rapide de problèmes complexes</li>
                        <li>Tech : Python, JavaScript, <span class="highlight">Infomaniak API</span></li>
                    </ul>
                </div>
            </section>
            
            <!-- Expérience -->
            <section>
                <h2 class="section-title">
                    <i class="fas fa-briefcase"></i>
                    Expérience Professionnelle
                </h2>
                
                <div class="experience-item">
                    <div class="exp-header">
                        <div>
                            <div class="exp-title">Software Developer</div>
                            <div class="exp-company">Innovatim - Temps plein</div>
                        </div>
                        <div class="exp-date">Oct. 2023 - Sept. 2024</div>
                    </div>
                    <ul class="exp-desc">
                        <li>Développement d'un logiciel IA en prenant en charge la <span class="highlight">conception des fonctionnalités</span> et la partie <span class="highlight">frontend</span></li>
                        <li>Conception d'architecture <span class="highlight">RAG (Retrieval Augmented Generation)</span> avec FAISS et intégration LLM</li>
                        <li>Travail en équipe sur site en Suisse</li>
                    </ul>
                </div>
            </section>
            
            <!-- Formation -->
            <section>
                <h2 class="section-title">
                    <i class="fas fa-graduation-cap"></i>
                    Formation
                </h2>
                
                <div class="experience-item">
                    <div class="exp-header">
                        <div>
                            <div class="exp-title">42 Lausanne</div>
                            <div class="exp-company">École d'Informatique</div>
                        </div>
                        <div class="exp-date">2024 - Présent</div>
                    </div>
                    <ul class="exp-desc">
                        <li>Formation intensive axée sur la <span class="highlight">résolution de problèmes complexes</span> et l'autonomie</li>
                        <li>Développement de projets bas niveau en <span class="highlight">C/C++</span> (gestion mémoire, performances, algorithmie)</li>
                        <li>Conception de systèmes complets et culture de la <span class="highlight">rigueur</span></li>
                        <li>Apprentissage par projets et <span class="highlight">peer-to-peer learning</span></li>
                    </ul>
                </div>
            </section>
        </div>
    </div>
</body>
</html>
