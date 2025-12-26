<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anusha K | Data Science Engineer</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Roboto+Mono:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #2563eb;
            --secondary: #7c3aed;
            --accent: #10b981;
            --dark: #1f2937;
            --light: #f9fafb;
            --gray: #6b7280;
            --card-bg: rgba(255, 255, 255, 0.1);
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
            color: var(--light);
            line-height: 1.6;
            overflow-x: hidden;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header Styles */
        header {
            text-align: center;
            padding: 40px 20px;
            margin-bottom: 40px;
            position: relative;
            overflow: hidden;
            border-radius: 20px;
            background: linear-gradient(135deg, rgba(37, 99, 235, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .floating-elements {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: -1;
        }

        .floating-element {
            position: absolute;
            width: 30px;
            height: 30px;
            background: rgba(37, 99, 235, 0.2);
            border-radius: 50%;
            animation: float 15s infinite linear;
        }

        .floating-element:nth-child(2) {
            top: 20%;
            left: 10%;
            width: 20px;
            height: 20px;
            background: rgba(124, 58, 237, 0.2);
            animation-delay: -5s;
        }

        .floating-element:nth-child(3) {
            top: 70%;
            left: 80%;
            width: 40px;
            height: 40px;
            background: rgba(16, 185, 129, 0.2);
            animation-delay: -10s;
        }

        .floating-element:nth-child(4) {
            top: 40%;
            left: 90%;
            width: 15px;
            height: 15px;
            animation-delay: -7s;
        }

        @keyframes float {
            0%, 100% {
                transform: translateY(0) rotate(0deg);
            }
            33% {
                transform: translateY(-30px) rotate(120deg);
            }
            66% {
                transform: translateY(20px) rotate(240deg);
            }
        }

        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid var(--primary);
            margin: 0 auto 20px;
            overflow: hidden;
            position: relative;
            box-shadow: 0 10px 30px rgba(37, 99, 235, 0.4);
            animation: pulse 3s infinite alternate;
        }

        @keyframes pulse {
            0% {
                box-shadow: 0 10px 30px rgba(37, 99, 235, 0.4);
            }
            100% {
                box-shadow: 0 10px 40px rgba(37, 99, 235, 0.7), 0 0 60px rgba(37, 99, 235, 0.2);
            }
        }

        .profile-img i {
            font-size: 70px;
            color: var(--primary);
            line-height: 150px;
            width: 100%;
            text-align: center;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: slideIn 1s ease-out;
        }

        .tagline {
            font-size: 1.3rem;
            color: var(--accent);
            margin-bottom: 20px;
            font-weight: 500;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 30px;
            flex-wrap: wrap;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 10px 20px;
            background: var(--card-bg);
            border-radius: 50px;
            transition: all 0.3s ease;
            cursor: pointer;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        .contact-item:hover {
            transform: translateY(-5px);
            background: rgba(37, 99, 235, 0.2);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }

        /* Section Styles */
        section {
            margin-bottom: 60px;
            animation: fadeInUp 1s ease-out;
        }

        .section-title {
            font-size: 2rem;
            margin-bottom: 30px;
            display: flex;
            align-items: center;
            gap: 15px;
            position: relative;
            padding-bottom: 10px;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), transparent);
            border-radius: 2px;
        }

        .section-title i {
            color: var(--primary);
        }

        /* Education & Info Card */
        .info-card {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 25px;
            margin-bottom: 25px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }

        .info-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
            border-color: rgba(37, 99, 235, 0.3);
        }

        .info-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.05), transparent);
            transition: left 0.7s ease;
        }

        .info-card:hover::before {
            left: 100%;
        }

        .info-card h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: var(--accent);
        }

        .info-card .subtitle {
            color: var(--gray);
            font-size: 1rem;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .info-card .cgpa {
            display: inline-block;
            padding: 5px 15px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            color: white;
            border-radius: 20px;
            font-weight: 600;
            font-size: 0.9rem;
            margin-top: 10px;
        }

        /* Toolbox */
        .toolbox-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }

        .tool-category {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 25px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .tool-category:hover {
            transform: translateY(-5px);
            border-color: rgba(16, 185, 129, 0.3);
        }

        .tool-category h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            color: var(--accent);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .tools {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
        }

        .tool {
            padding: 8px 15px;
            background: rgba(37, 99, 235, 0.1);
            border-radius: 10px;
            font-size: 0.9rem;
            border: 1px solid rgba(37, 99, 235, 0.2);
            transition: all 0.3s ease;
            cursor: default;
        }

        .tool:hover {
            background: rgba(37, 99, 235, 0.3);
            transform: scale(1.05);
        }

        /* Achievements */
        .achievements-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 25px;
        }

        .achievement-card {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 25px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }

        .achievement-card:hover {
            transform: translateY(-10px);
            border-color: rgba(124, 58, 237, 0.3);
        }

        .achievement-card h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
            color: var(--accent);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .achievement-card p {
            color: var(--gray);
            margin-bottom: 15px;
        }

        .achievement-icon {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
            font-size: 1.5rem;
        }

        /* Animations */
        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
            .section-title {
                font-size: 1.7rem;
            }
            
            .contact-info {
                flex-direction: column;
                align-items: center;
            }
            
            .toolbox-container, .achievements-container {
                grid-template-columns: 1fr;
            }
            
            .info-card, .tool-category, .achievement-card {
                padding: 20px;
            }
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px 0;
            margin-top: 40px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: var(--gray);
            font-size: 0.9rem;
        }

        .social-icons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .social-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: var(--card-bg);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.3rem;
            transition: all 0.3s ease;
            color: var(--light);
            text-decoration: none;
        }

        .social-icon:hover {
            background: var(--primary);
            transform: translateY(-5px) rotate(10deg);
        }

        /* Typing Effect */
        .typing-container {
            height: 40px;
            margin: 20px 0;
            display: flex;
            justify-content: center;
        }

        .typing-text {
            overflow: hidden;
            border-right: 3px solid var(--primary);
            white-space: nowrap;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
            font-family: 'Roboto Mono', monospace;
            font-size: 1.2rem;
        }

        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: var(--primary) }
        }

        /* Particle background */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            pointer-events: none;
        }
    </style>
</head>
<body>
    <!-- Particle Background -->
    <div class="particles" id="particles"></div>
    
    <div class="container">
        <header>
            <div class="floating-elements">
                <div class="floating-element"></div>
                <div class="floating-element"></div>
                <div class="floating-element"></div>
                <div class="floating-element"></div>
            </div>
            
            <div class="profile-img">
                <i class="fas fa-user-circle"></i>
            </div>
            
            <h1>Anusha K</h1>
            <div class="tagline">Data Science Engineer | AI/ML Researcher</div>
            
            <div class="typing-container">
                <div class="typing-text">Specializing in ML, DL, NLP & Generative AI</div>
            </div>
            
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fas fa-graduation-cap"></i>
                    <span>B.Tech in Computer Science (Data Science)</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <span>Tirupati, India</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <span>anushakprn@gmail.com</span>
                </div>
            </div>
        </header>

        <section>
            <h2 class="section-title"><i class="fas fa-user-graduate"></i> Education</h2>
            <div class="info-card">
                <h3>Mohan Babu University</h3>
                <div class="subtitle"><i class="fas fa-university"></i> B.Tech in Computer Science (Data Science)</div>
                <p>Specialized in Data Science with a focus on Machine Learning, Deep Learning, and AI technologies.</p>
                <div class="cgpa">CGPA: 9.69</div>
            </div>
        </section>

        <section>
            <h2 class="section-title"><i class="fas fa-toolbox"></i> My Toolbox</h2>
            <div class="toolbox-container">
                <div class="tool-category">
                    <h3><i class="fas fa-code"></i> Languages & Tools</h3>
                    <div class="tools">
                        <div class="tool">Python</div>
                        <div class="tool">SQL</div>
                        <div class="tool">Java</div>
                        <div class="tool">C++</div>
                        <div class="tool">Git</div>
                        <div class="tool">Docker</div>
                        <div class="tool">Linux</div>
                    </div>
                </div>
                
                <div class="tool-category">
                    <h3><i class="fas fa-brain"></i> Machine Learning & AI</h3>
                    <div class="tools">
                        <div class="tool">TensorFlow</div>
                        <div class="tool">PyTorch</div>
                        <div class="tool">Scikit-learn</div>
                        <div class="tool">Keras</div>
                        <div class="tool">OpenCV</div>
                        <div class="tool">NLTK</div>
                        <div class="tool">Transformers</div>
                        <div class="tool">LangChain</div>
                    </div>
                </div>
                
                <div class="tool-category">
                    <h3><i class="fas fa-chart-bar"></i> Data Analysis & BI</h3>
                    <div class="tools">
                        <div class="tool">Pandas</div>
                        <div class="tool">NumPy</div>
                        <div class="tool">Matplotlib</div>
                        <div class="tool">Seaborn</div>
                        <div class="tool">Plotly</div>
                        <div class="tool">Tableau</div>
                        <div class="tool">Power BI</div>
                    </div>
                </div>
                
                <div class="tool-category">
                    <h3><i class="fas fa-laptop-code"></i> IDEs & Platforms</h3>
                    <div class="tools">
                        <div class="tool">Jupyter</div>
                        <div class="tool">VS Code</div>
                        <div class="tool">Google Colab</div>
                        <div class="tool">AWS</div>
                        <div class="tool">Azure</div>
                        <div class="tool">GitHub</div>
                    </div>
                </div>
            </div>
        </section>

        <section>
            <h2 class="section-title"><i class="fas fa-certificate"></i> Certifications</h2>
            <div class="achievements-container">
                <div class="achievement-card">
                    <div class="achievement-icon">
                        <i class="fab fa-google"></i>
                    </div>
                    <h3>Google Advanced Data Analytics</h3>
                    <p>Mastered advanced data analytics techniques and tools for data-driven decision making.</p>
                </div>
                
                <div class="achievement-card">
                    <div class="achievement-icon">
                        <i class="fab fa-ibm"></i>
                    </div>
                    <h3>IBM Python for Data Science and AI</h3>
                    <p>Python programming for data science, machine learning, and artificial intelligence applications.</p>
                </div>
                
                <div class="achievement-card">
                    <div class="achievement-icon">
                        <i class="fab fa-aws"></i>
                    </div>
                    <h3>AWS Solution Architecture</h3>
                    <p>Job simulation focusing on designing scalable and reliable applications on AWS.</p>
                </div>
            </div>
        </section>

        <section>
            <h2 class="section-title"><i class="fas fa-trophy"></i> Achievements & Roles</h2>
            <div class="achievements-container">
                <div class="achievement-card">
                    <h3><i class="fas fa-file-alt"></i> Published Research Paper</h3>
                    <p><strong>BERT vs. RoBERTa for e-commerce attribute prediction</strong> - Comparative analysis of transformer models for e-commerce applications.</p>
                </div>
                
                <div class="achievement-card">
                    <h3><i class="fas fa-users"></i> IEEE Computer Society Secretary</h3>
                    <p>Led multiple technical sessions and organized workshops for 100+ members.</p>
                </div>
                
                <div class="achievement-card">
                    <h3><i class="fas fa-hands-helping"></i> GDSC-MBU Coordinator</h3>
                    <p>Mentored peers and organized machine learning workshops and hackathons.</p>
                </div>
                
                <div class="achievement-card">
                    <h3><i class="fas fa-laptop-code"></i> ML Intern - The Idea Gen Technologies</h3>
                    <p>Developed NLP & Predictive Maintenance models with high accuracy metrics.</p>
                </div>
                
                <div class="achievement-card">
                    <h3><i class="fas fa-female"></i> Girlscript Contributor</h3>
                    <p>Summer of Code Contributor & Campus Ambassador promoting tech education.</p>
                </div>
            </div>
        </section>

        <footer>
            <p>Connect with me</p>
            <div class="social-icons">
                <a href="#" class="social-icon" title="LinkedIn">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="#" class="social-icon" title="GitHub">
                    <i class="fab fa-github"></i>
                </a>
                <a href="#" class="social-icon" title="Email">
                    <i class="fas fa-envelope"></i>
                </a>
                <a href="#" class="social-icon" title="Research">
                    <i class="fas fa-file-pdf"></i>
                </a>
            </div>
            <p style="margin-top: 20px;">&copy; 2023 Anusha K | Data Science Engineer</p>
            <p>Portfolio README with Advanced Animations</p>
        </footer>
    </div>

    <script>
        // Create particle background
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('floating-element');
                
                // Random size
                const size = Math.random() * 20 + 5;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                
                // Random position
                particle.style.left = `${Math.random() * 100}%`;
                particle.style.top = `${Math.random() * 100}%`;
                
                // Random color
                const colors = [
                    'rgba(37, 99, 235, 0.2)',
                    'rgba(124, 58, 237, 0.2)',
                    'rgba(16, 185, 129, 0.2)',
                    'rgba(239, 68, 68, 0.2)'
                ];
                particle.style.background = colors[Math.floor(Math.random() * colors.length)];
                
                // Random animation
                const duration = Math.random() * 20 + 10;
                const delay = Math.random() * -20;
                particle.style.animation = `float ${duration}s infinite linear ${delay}s`;
                
                particlesContainer.appendChild(particle);
            }
        }
        
        // Add hover effects to cards
        function addCardHoverEffects() {
            const cards = document.querySelectorAll('.info-card, .tool-category, .achievement-card');
            
            cards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    const allCards = document.querySelectorAll('.info-card, .tool-category, .achievement-card');
                    allCards.forEach(otherCard => {
                        if (otherCard !== this) {
                            otherCard.style.opacity = '0.7';
                            otherCard.style.transform = 'scale(0.98)';
                        }
                    });
                });
                
                card.addEventListener('mouseleave', function() {
                    const allCards = document.querySelectorAll('.info-card, .tool-category, .achievement-card');
                    allCards.forEach(otherCard => {
                        otherCard.style.opacity = '1';
                        otherCard.style.transform = 'scale(1)';
                    });
                });
            });
        }
        
        // Typing text animation
        function initTypingEffect() {
            const texts = [
                "Specializing in ML, DL, NLP & Generative AI",
                "Results-driven Data Science Engineer",
                "Published Researcher | IEEE Leader",
                "Hands-on experience in AI/ML technologies"
            ];
            
            let textIndex = 0;
            const typingElement = document.querySelector('.typing-text');
            
            function typeText() {
                const currentText = texts[textIndex];
                typingElement.textContent = '';
                typingElement.style.animation = 'none';
                
                setTimeout(() => {
                    typingElement.textContent = currentText;
                    typingElement.style.animation = 'typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite';
                    
                    textIndex = (textIndex + 1) % texts.length;
                    
                    setTimeout(typeText, 4000);
                }, 500);
            }
            
            typeText();
        }
        
        // Initialize everything when page loads
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            addCardHoverEffects();
            initTypingEffect();
            
            // Add click effects to contact items
            document.querySelectorAll('.contact-item').forEach(item => {
                item.addEventListener('click', function() {
                    this.style.transform = 'scale(0.95)';
                    setTimeout(() => {
                        this.style.transform = '';
                    }, 300);
                });
            });
        });
    </script>
</body>
</html>
