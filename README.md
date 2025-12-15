# Yessica-dominguez.github.iou
Crea mi página web
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yessica Lizbeth Domínguez Carmona - UACM</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #ec4899 0%, #a855f7 100%);
            min-height: 100vh;
            color: #333;
        }

        /* Navegación */
        nav {
            background: rgba(255, 255, 255, 0.95);
            padding: 1rem 2rem;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
        }

        nav a {
            text-decoration: none;
            color: #ec4899;
            font-weight: 600;
            transition: color 0.3s;
            padding: 0.5rem 1rem;
        }

        nav a:hover {
            color: #a855f7;
        }

        /* Header con animación de colores */
        header {
            margin-top: 80px;
            padding: 3rem 2rem;
            text-align: center;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #f7b731);
            background-size: 400% 400%;
            animation: gradientShift 8s ease infinite;
            color: white;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
            animation: fadeInDown 1s ease;
        }

        header p {
            font-size: 1.2rem;
            animation: fadeInUp 1s ease 0.3s both;
        }

        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Container principal */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* Secciones */
        section {
            background: white;
            margin: 2rem 0;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            animation: fadeIn 1s ease;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        section h2 {
            color: #ec4899;
            margin-bottom: 1.5rem;
            font-size: 2rem;
            border-bottom: 3px solid #a855f7;
            padding-bottom: 0.5rem;
        }

        /* Sección de información personal */
        .info-personal {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .info-personal i {
            color: #ec4899;
            font-size: 1.5rem;
        }

        /* Redes sociales */
        .redes-sociales {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .redes-sociales a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, #ec4899 0%, #a855f7 100%);
            color: white;
            border-radius: 50%;
            text-decoration: none;
            font-size: 1.5rem;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .redes-sociales a:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        /* Ubicación institucional */
        .ubicacion {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 2rem;
            border-radius: 15px;
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .ubicacion i {
            font-size: 3rem;
        }

        /* Grid de IA */
        .ia-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }

        .ia-card {
            background: linear-gradient(135deg, #ec4899 0%, #a855f7 100%);
            color: white;
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s;
            cursor: pointer;
        }

        .ia-card:hover {
            transform: scale(1.05);
        }

        .ia-card i {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .ia-card h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }

        /* Formulario de contacto */
        .contact-form {
            display: grid;
            gap: 1rem;
        }

        .form-group {
            display: flex;
            flex-direction: column;
        }

        .form-group label {
            margin-bottom: 0.5rem;
            color: #ec4899;
            font-weight: 600;
        }

        .form-group input,
        .form-group textarea {
            padding: 0.8rem;
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            font-family: 'Poppins', sans-serif;
            transition: border-color 0.3s;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #ec4899;
        }

        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }

        .submit-btn {
            background: linear-gradient(135deg, #ec4899 0%, #a855f7 100%);
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .submit-btn:hover {
            transform: translateY(-2px);
        }

        /* Video y multimedia */
        .multimedia-container {
            display: grid;
            gap: 2rem;
            margin-top: 1.5rem;
        }

        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            border-radius: 15px;
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border-radius: 15px;
        }

        .image-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
        }

        .image-gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            transition: transform 0.3s;
        }

        .image-gallery img:hover {
            transform: scale(1.05);
        }

        /* Footer */
        footer {
            background: rgba(255, 255, 255, 0.95);
            text-align: center;
            padding: 2rem;
            margin-top: 2rem;
        }

        footer p {
            color: #ec4899;
            font-weight: 600;
        }

        /* Responsive */
        @media (max-width: 768px) {
            header h1 {
                font-size: 1.8rem;
            }

            nav ul {
                gap: 1rem;
            }

            .ia-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Navegación -->
    <nav>
        <ul>
            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#chatgpt">ChatGPT</a></li>
            <li><a href="#claude">Claude</a></li>
            <li><a href="#deepseek">DeepSeek</a></li>
            <li><a href="#quora">Quora</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
    </nav>

    <!-- Header con animación -->
    <header id="inicio">
        <h1>Yessica Lizbeth Domínguez Carmona</h1>
        <p>Universidad Autónoma de la Ciudad de México</p>
    </header>

    <div class="container">
        <!-- Información Personal -->
        <section>
            <h2><i class="fas fa-user"></i> Información Personal</h2>
            <div class="info-personal">
                <i class="fas fa-envelope"></i>
                <p><strong>Correo Institucional:</strong> yessica.lizbeth.dominguez.carmona@estudiantxs.uacm.edu.mx</p>
            </div>
            <div class="info-personal">
                <i class="fas fa-graduation-cap"></i>
                <p><strong>Institución:</strong> Universidad Autónoma de la Ciudad de México</p>
            </div>
        </section>

        <!-- Ubicación Institucional -->
        <section>
            <div class="ubicacion">
                <i class="fas fa-map-marker-alt"></i>
                <div>
                    <h3>UACM Plantel Casa Libertad</h3>
                    <p>Encuentra tu camino hacia el conocimiento en nuestro campus</p>
                </div>
            </div>
        </section>

        <!-- Redes Sociales -->
        <section>
            <h2><i class="fas fa-share-alt"></i> Sígueme en Redes Sociales</h2>
            <div class="redes-sociales">
                <a href="https://www.facebook.com/profile.php?id=yessicadc" target="_blank" title="Facebook - Yessica dc">
                    <i class="fab fa-facebook-f"></i>
                </a>
                <a href="https://www.threads.net/@yessica_car5" target="_blank" title="Threads - @yessica_car5">
                    <i class="fab fa-twitter"></i>
                </a>
                <a href="https://www.instagram.com/yessica_car5?igsh=MXJvbTZ4eGhoZnM5OQ==" target="_blank" title="Instagram - @yessica_car5">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="https://www.linkedin.com" target="_blank" title="LinkedIn">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="https://www.github.com" target="_blank" title="GitHub">
                    <i class="fab fa-github"></i>
                </a>
                <a href="https://wa.me" target="_blank" title="WhatsApp">
                    <i class="fab fa-whatsapp"></i>
                </a>
            </div>
        </section>

        <!-- Secciones de IA -->
        <section id="chatgpt">
            <h2><i class="fas fa-robot"></i> ChatGPT</h2>
            <div style="text-align: center; margin-bottom: 2rem;">
                <button id="confettiBtn" style="background: linear-gradient(135deg, #ec4899 0%, #a855f7 100%); color: white; padding: 1rem 2rem; border: none; border-radius: 8px; font-size: 1rem; font-weight: 600; cursor: pointer; transition: transform 0.3s;">
                    🎉 ¡Lanzar Confeti!
                </button>
            </div>
            <canvas id="confettiCanvas" style="position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: 9999;"></canvas>
            <div class="ia-grid">
                <div class="ia-card">
                    <i class="fas fa-brain"></i>
                    <h3>Inteligencia Artificial</h3>
                    <p>ChatGPT es un modelo de lenguaje desarrollado por OpenAI capaz de mantener conversaciones naturales y ayudar en diversas tareas.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-comments"></i>
                    <h3>Conversaciones</h3>
                    <p>Puede responder preguntas, generar contenido creativo y asistir en tareas de programación.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-lightbulb"></i>
                    <h3>Aplicaciones</h3>
                    <p>Usado en educación, desarrollo de software, escritura creativa y mucho más.</p>
                </div>
            </div>
        </section>

        <section id="claude">
            <h2><i class="fas fa-robot"></i> Claude</h2>
            <div class="ia-grid">
                <div class="ia-card">
                    <i class="fas fa-shield-alt"></i>
                    <h3>Seguro y Confiable</h3>
                    <p>Claude es un asistente de IA desarrollado por Anthropic, enfocado en ser útil, honesto e inofensivo.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-book"></i>
                    <h3>Análisis Profundo</h3>
                    <p>Capaz de procesar documentos largos y proporcionar análisis detallados.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-code"></i>
                    <h3>Asistente de Código</h3>
                    <p>Ayuda en el desarrollo de software con sugerencias precisas y seguras.</p>
                </div>
            </div>
        </section>

        <section id="deepseek">
            <h2><i class="fas fa-search"></i> DeepSeek</h2>
            <div class="ia-grid">
                <div class="ia-card">
                    <i class="fas fa-database"></i>
                    <h3>Búsqueda Avanzada</h3>
                    <p>DeepSeek es una herramienta de búsqueda profunda que utiliza IA para encontrar información relevante.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-chart-line"></i>
                    <h3>Análisis de Datos</h3>
                    <p>Procesa grandes volúmenes de información para extraer insights valiosos.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-network-wired"></i>
                    <h3>Conexiones</h3>
                    <p>Identifica patrones y relaciones entre diferentes conjuntos de datos.</p>
                </div>
            </div>
        </section>

        <section id="quora">
            <h2><i class="fas fa-question-circle"></i> Quora</h2>
            <div class="ia-grid">
                <div class="ia-card">
                    <i class="fas fa-users"></i>
                    <h3>Comunidad Global</h3>
                    <p>Quora es una plataforma donde millones de personas comparten conocimiento respondiendo preguntas.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-graduation-cap"></i>
                    <h3>Aprendizaje</h3>
                    <p>Accede a respuestas de expertos en diversos campos del conocimiento.</p>
                </div>
                <div class="ia-card">
                    <i class="fas fa-share"></i>
                    <h3>Comparte</h3>
                    <p>Contribuye con tu experiencia y ayuda a otros a resolver sus dudas.</p>
                </div>
            </div>
        </section>

        <!-- Multimedia -->
        <section>
            <h2><i class="fas fa-photo-video"></i> Multimedia</h2>
            <div class="multimedia-container">
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
                <div class="image-gallery">
                    <img src="https://via.placeholder.com/300x200/667eea/ffffff?text=IA+Imagen+1" alt="Inteligencia Artificial 1">
                    <img src="https://via.placeholder.com/300x200/764ba2/ffffff?text=IA+Imagen+2" alt="Inteligencia Artificial 2">
                    <img src="https://via.placeholder.com/300x200/f093fb/ffffff?text=IA+Imagen+3" alt="Inteligencia Artificial 3">
                </div>
            </div>
        </section>

        <!-- Formulario de Contacto -->
        <section id="contacto">
            <h2><i class="fas fa-envelope"></i> Contacto</h2>
            <form class="contact-form">
                <div class="form-group">
                    <label for="nombre">Nombre Completo</label>
                    <input type="text" id="nombre" name="nombre" required>
                </div>
                <div class="form-group">
                    <label for="email">Correo Electrónico</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="asunto">Asunto</label>
                    <input type="text" id="asunto" name="asunto" required>
                </div>
                <div class="form-group">
                    <label for="mensaje">Mensaje</label>
                    <textarea id="mensaje" name="mensaje" required></textarea>
                </div>
                <button type="submit" class="submit-btn">
                    <i class="fas fa-paper-plane"></i> Enviar Mensaje
                </button>
            </form>
        </section>
    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Yessica Lizbeth Domínguez Carmona - Universidad Autónoma de la Ciudad de México</p>
        <p>Computación II - Proyecto Web</p>
    </footer>

    <script>
        // Smooth scroll para navegación
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                target.scrollIntoView({ behavior: 'smooth', block: 'start' });
            });
        });

        // Formulario
        document.querySelector('.contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('¡Gracias por tu mensaje! Te contactaremos pronto.');
            this.reset();
        });

        // Efecto de Confeti
        const canvas = document.getElementById('confettiCanvas');
        const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        let confettiPieces = [];

        class Confetti {
            constructor() {
                this.x = Math.random() * canvas.width;
                this.y = -20;
                this.size = Math.random() * 10 + 5;
                this.speedY = Math.random() * 3 + 2;
                this.speedX = Math.random() * 2 - 1;
                this.color = `hsl(${Math.random() * 360}, 100%, 50%)`;
                this.rotation = Math.random() * 360;
                this.rotationSpeed = Math.random() * 5 - 2.5;
            }

            update() {
                this.y += this.speedY;
                this.x += this.speedX;
                this.rotation += this.rotationSpeed;

                if (this.y > canvas.height) {
                    return false;
                }
                return true;
            }

            draw() {
                ctx.save();
                ctx.translate(this.x, this.y);
                ctx.rotate((this.rotation * Math.PI) / 180);
                ctx.fillStyle = this.color;
                ctx.fillRect(-this.size / 2, -this.size / 2, this.size, this.size);
                ctx.restore();
            }
        }

        function createConfetti() {
            for (let i = 0; i < 100; i++) {
                confettiPieces.push(new Confetti());
            }
        }

        function animateConfetti() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            
            confettiPieces = confettiPieces.filter(confetti => {
                confetti.draw();
                return confetti.update();
            });

            if (confettiPieces.length > 0) {
                requestAnimationFrame(animateConfetti);
            }
        }

        document.getElementById('confettiBtn').addEventListener('click', function() {
            createConfetti();
            animateConfetti();
            this.style.transform = 'scale(0.95)';
            setTimeout(() => {
                this.style.transform = 'scale(1)';
            }, 100);
        });

        window.addEventListener('resize', () => {
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
        });
    </script>
</body>
</html>
