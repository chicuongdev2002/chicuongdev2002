<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CuongDev - Cosmic Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #0a0a1f 0%, #1a0a2e 50%, #2a0a3e 100%);
            color: #ffffff;
            overflow-x: hidden;
            position: relative;
            min-height: 100vh;
        }

        /* Starfield Background */
        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }

        .star {
            position: absolute;
            background: white;
            border-radius: 50%;
            animation: twinkle 3s infinite;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.3; }
            50% { opacity: 1; }
        }

        /* Shooting Stars / Meteors */
        .meteor {
            position: fixed;
            top: -50px;
            left: 100%;
            width: 2px;
            height: 80px;
            background: linear-gradient(to bottom, rgba(255, 255, 255, 1), transparent);
            transform: rotate(-45deg);
            animation: shootingStar 3s linear infinite;
            box-shadow: 0 0 10px rgba(255, 255, 255, 0.8);
        }

        .meteor::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to bottom, #667eea, #764ba2, #f093fb);
            filter: blur(8px);
        }

        @keyframes shootingStar {
            0% {
                transform: translate(0, 0) rotate(-45deg);
                opacity: 1;
            }
            100% {
                transform: translate(-1500px, 1500px) rotate(-45deg);
                opacity: 0;
            }
        }

        .meteor:nth-child(1) { animation-delay: 0s; top: 10%; }
        .meteor:nth-child(2) { animation-delay: 1.5s; top: 25%; }
        .meteor:nth-child(3) { animation-delay: 3s; top: 40%; }
        .meteor:nth-child(4) { animation-delay: 4.5s; top: 15%; }
        .meteor:nth-child(5) { animation-delay: 6s; top: 35%; }

        /* Container */
        .container {
            position: relative;
            z-index: 1;
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* Header */
        header {
            text-align: center;
            padding: 60px 20px;
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            margin-bottom: 40px;
            box-shadow: 0 8px 32px rgba(102, 126, 234, 0.2);
            animation: fadeInDown 1s ease-out;
        }

        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h1 {
            font-size: 4em;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 20px;
            text-shadow: 0 0 40px rgba(102, 126, 234, 0.5);
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from {
                filter: drop-shadow(0 0 20px rgba(102, 126, 234, 0.5));
            }
            to {
                filter: drop-shadow(0 0 40px rgba(240, 147, 251, 0.8));
            }
        }

        .tagline {
            font-size: 1.5em;
            color: #a8b2d1;
            margin-top: 10px;
        }

        /* Cards */
        .card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 30px;
            margin-bottom: 30px;
            transition: all 0.3s ease;
            animation: fadeInUp 1s ease-out;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .card:hover {
            transform: translateY(-10px);
            border-color: rgba(102, 126, 234, 0.5);
            box-shadow: 0 15px 50px rgba(102, 126, 234, 0.3);
        }

        h2 {
            color: #667eea;
            font-size: 2.5em;
            margin-bottom: 20px;
            text-align: center;
        }

        /* Tech Stack */
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .tech-item {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.1), rgba(240, 147, 251, 0.1));
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .tech-item:hover {
            transform: scale(1.1);
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.2), rgba(240, 147, 251, 0.2));
            box-shadow: 0 0 30px rgba(102, 126, 234, 0.4);
        }

        /* Stats */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .stat-box {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.2), rgba(118, 75, 162, 0.2));
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }

        .stat-box:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 40px rgba(102, 126, 234, 0.4);
        }

        .stat-number {
            font-size: 3em;
            font-weight: bold;
            background: linear-gradient(135deg, #667eea, #f093fb);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .stat-label {
            margin-top: 10px;
            color: #a8b2d1;
            font-size: 1.2em;
        }

        /* Social Links */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 30px;
        }

        .social-btn {
            padding: 15px 30px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            border: none;
            border-radius: 50px;
            color: white;
            font-size: 1.1em;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
        }

        .social-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 0 30px rgba(102, 126, 234, 0.6);
            background: linear-gradient(135deg, #764ba2, #f093fb);
        }

        /* Planet Animation */
        .planet {
            position: fixed;
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background: radial-gradient(circle at 30% 30%, #667eea, #764ba2);
            box-shadow: 0 0 50px rgba(102, 126, 234, 0.5);
            animation: float 6s ease-in-out infinite;
            z-index: 0;
        }

        .planet1 { top: 10%; right: 10%; animation-delay: 0s; }
        .planet2 { bottom: 20%; left: 10%; animation-delay: 2s; width: 80px; height: 80px; }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-30px); }
        }

        /* Responsive */
        @media (max-width: 768px) {
            h1 { font-size: 2.5em; }
            h2 { font-size: 2em; }
            .tagline { font-size: 1.2em; }
        }
    </style>
</head>
<body>
    <!-- Stars Background -->
    <div class="stars" id="stars"></div>

    <!-- Shooting Stars / Meteors -->
    <div class="meteor"></div>
    <div class="meteor"></div>
    <div class="meteor"></div>
    <div class="meteor"></div>
    <div class="meteor"></div>

    <!-- Planets -->
    <div class="planet planet1"></div>
    <div class="planet planet2"></div>

    <!-- Main Content -->
    <div class="container">
        <header>
            <h1>🚀 CUONG DEV</h1>
            <p class="tagline">Fullstack Developer | AI Engineer | Blockchain Expert</p>
            <p style="margin-top: 20px; color: #a8b2d1;">
                Building the future with AI & Blockchain ✨
            </p>
        </header>

        <div class="card">
            <h2>🧠 About Me</h2>
            <p style="font-size: 1.2em; line-height: 1.8; color: #a8b2d1; text-align: center;">
                Passionate developer from Ho Chi Minh City, Vietnam 🇻🇳<br>
                Specializing in AI, Blockchain, and Full-stack Development<br>
                Always exploring new technologies and building innovative solutions
            </p>
        </div>

        <div class="card">
            <h2>🛠️ Tech Stack</h2>
            <div class="tech-grid">
                <div class="tech-item">⚛️ React</div>
                <div class="tech-item">📱 Next.js</div>
                <div class="tech-item">🟢 Node.js</div>
                <div class="tech-item">🔷 TypeScript</div>
                <div class="tech-item">🐍 Python</div>
                <div class="tech-item">🔗 Blockchain</div>
                <div class="tech-item">🤖 AI/ML</div>
                <div class="tech-item">🗄️ PostgreSQL</div>
                <div class="tech-item">⚡ Supabase</div>
                <div class="tech-item">🐳 Docker</div>
                <div class="tech-item">☁️ AWS</div>
                <div class="tech-item">🎨 TailwindCSS</div>
            </div>
        </div>

        <div class="card">
            <h2>📊 GitHub Stats</h2>
            <div class="stats-grid">
                <div class="stat-box">
                    <div class="stat-number">50+</div>
                    <div class="stat-label">Projects</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">1000+</div>
                    <div class="stat-label">Commits</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">500+</div>
                    <div class="stat-label">Contributions</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">10+</div>
                    <div class="stat-label">Languages</div>
                </div>
            </div>
        </div>

        <div class="card">
            <h2>🎯 Current Focus</h2>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 20px;">
                <div style="text-align: center; padding: 20px;">
                    <div style="font-size: 3em;">🤖</div>
                    <h3 style="color: #667eea; margin: 10px 0;">AI Development</h3>
                    <p style="color: #a8b2d1;">Building intelligent systems</p>
                </div>
                <div style="text-align: center; padding: 20px;">
                    <div style="font-size: 3em;">⛓️</div>
                    <h3 style="color: #764ba2; margin: 10px 0;">Blockchain</h3>
                    <p style="color: #a8b2d1;">Smart contracts & DApps</p>
                </div>
                <div style="text-align: center; padding: 20px;">
                    <div style="font-size: 3em;">🏗️</div>
                    <h3 style="color: #f093fb; margin: 10px 0;">System Design</h3>
                    <p style="color: #a8b2d1;">Scalable architectures</p>
                </div>
                <div style="text-align: center; padding: 20px;">
                    <div style="font-size: 3em;">🌟</div>
                    <h3 style="color: #667eea; margin: 10px 0;">Open Source</h3>
                    <p style="color: #a8b2d1;">Contributing to community</p>
                </div>
            </div>
        </div>

        <div class="card">
            <h2>📫 Connect With Me</h2>
            <div class="social-links">
                <a href="https://github.com/chicuongdev2002" class="social-btn" target="_blank">
                    GitHub
                </a>
                <a href="https://linkedin.com/in/chicuongdev" class="social-btn" target="_blank">
                    LinkedIn
                </a>
                <a href="https://twitter.com/chicuongdev" class="social-btn" target="_blank">
                    Twitter
                </a>
                <a href="mailto:chicuongdev2002@gmail.com" class="social-btn">
                    Email
                </a>
                <a href="https://t.me/chicuongdev" class="social-btn" target="_blank">
                    Telegram
                </a>
            </div>
        </div>

        <div style="text-align: center; margin-top: 50px; padding: 30px; color: #a8b2d1;">
            <p style="font-size: 1.3em; font-style: italic;">
                "In the vast universe of code, every bug is a new star to discover" 🌌
            </p>
            <p style="margin-top: 20px;">
                Made with 💜 by CuongDev
            </p>
        </div>
    </div>

    <script>
        // Generate random stars
        const starsContainer = document.getElementById('stars');
        for (let i = 0; i < 200; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            star.style.width = Math.random() * 3 + 'px';
            star.style.height = star.style.width;
            star.style.left = Math.random() * 100 + '%';
            star.style.top = Math.random() * 100 + '%';
            star.style.animationDelay = Math.random() * 3 + 's';
            starsContainer.appendChild(star);
        }

        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
