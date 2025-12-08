<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CuongDev | GitHub Profile Dashboard</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Fira Code', 'Courier New', monospace;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%);
            color: #00ff9c;
            min-height: 100vh;
            padding: 20px;
            overflow-x: hidden;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .header {
            text-align: center;
            padding: 40px 20px;
            background: linear-gradient(90deg, #000000 0%, #0f0f0f 50%, #000000 100%);
            border: 2px solid #00ff9c;
            border-radius: 20px;
            margin-bottom: 40px;
            box-shadow: 0 0 40px rgba(0, 255, 156, 0.3);
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from {
                box-shadow: 0 0 20px rgba(0, 255, 156, 0.2);
            }
            to {
                box-shadow: 0 0 40px rgba(0, 255, 156, 0.5);
            }
        }

        .header h1 {
            font-size: 3em;
            text-shadow: 0 0 20px #00ff9c;
            margin-bottom: 10px;
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.7; }
        }

        .header .tagline {
            font-size: 1.2em;
            color: #00dd88;
            margin-top: 10px;
        }

        .loading {
            text-align: center;
            padding: 50px;
            font-size: 1.5em;
            color: #00ff9c;
        }

        .spinner {
            border: 4px solid rgba(0, 255, 156, 0.1);
            border-top: 4px solid #00ff9c;
            border-radius: 50%;
            width: 60px;
            height: 60px;
            animation: spin 1s linear infinite;
            margin: 20px auto;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        .profile-section {
            display: grid;
            grid-template-columns: 350px 1fr;
            gap: 30px;
            margin-bottom: 40px;
        }

        @media (max-width: 968px) {
            .profile-section {
                grid-template-columns: 1fr;
            }
        }

        .profile-card {
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%);
            border: 2px solid #00ff9c;
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 0 30px rgba(0, 255, 156, 0.2);
            text-align: center;
        }

        .avatar {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 4px solid #00ff9c;
            margin: 0 auto 20px;
            box-shadow: 0 0 30px rgba(0, 255, 156, 0.5);
            object-fit: cover;
        }

        .profile-name {
            font-size: 2em;
            margin-bottom: 10px;
            text-shadow: 0 0 10px #00ff9c;
        }

        .profile-bio {
            color: #00dd88;
            margin: 15px 0;
            line-height: 1.6;
        }

        .profile-stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-top: 20px;
        }

        .stat-box {
            background: #0a0a0a;
            padding: 15px;
            border-radius: 10px;
            border: 1px solid #00ff9c;
            transition: all 0.3s;
        }

        .stat-box:hover {
            background: #1a1a1a;
            box-shadow: 0 0 20px rgba(0, 255, 156, 0.3);
            transform: translateY(-5px);
        }

        .stat-number {
            font-size: 2em;
            font-weight: bold;
            color: #00ff9c;
        }

        .stat-label {
            font-size: 0.9em;
            color: #00dd88;
            margin-top: 5px;
        }

        .info-card {
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%);
            border: 2px solid #00ff9c;
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 0 30px rgba(0, 255, 156, 0.2);
        }

        .info-card h2 {
            font-size: 1.8em;
            margin-bottom: 20px;
            text-shadow: 0 0 10px #00ff9c;
            border-bottom: 2px solid #00ff9c;
            padding-bottom: 10px;
        }

        .info-item {
            display: flex;
            align-items: center;
            margin: 15px 0;
            padding: 10px;
            background: #0a0a0a;
            border-radius: 8px;
            border: 1px solid #00ff9c33;
        }

        .info-item strong {
            color: #00ff9c;
            margin-right: 10px;
            min-width: 120px;
        }

        .repos-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 25px;
            margin-top: 40px;
        }

        .repo-card {
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%);
            border: 2px solid #00ff9c;
            border-radius: 15px;
            padding: 25px;
            transition: all 0.3s;
            cursor: pointer;
            box-shadow: 0 0 20px rgba(0, 255, 156, 0.1);
        }

        .repo-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 0 40px rgba(0, 255, 156, 0.4);
            border-color: #00ffcc;
        }

        .repo-name {
            font-size: 1.5em;
            color: #00ff9c;
            margin-bottom: 10px;
            text-shadow: 0 0 5px #00ff9c;
        }

        .repo-description {
            color: #00dd88;
            margin: 10px 0;
            line-height: 1.5;
        }

        .repo-stats {
            display: flex;
            gap: 20px;
            margin-top: 15px;
            font-size: 0.9em;
        }

        .repo-stat {
            display: flex;
            align-items: center;
            gap: 5px;
            color: #00ff9c;
        }

        .language-tag {
            display: inline-block;
            background: #00ff9c22;
            color: #00ff9c;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85em;
            margin-top: 10px;
            border: 1px solid #00ff9c55;
        }

        .error {
            background: #ff000022;
            border: 2px solid #ff0000;
            color: #ff6666;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            margin: 20px 0;
        }

        .section-title {
            font-size: 2.5em;
            text-align: center;
            margin: 40px 0 30px;
            text-shadow: 0 0 20px #00ff9c;
            animation: pulse 2s ease-in-out infinite;
        }

        .btn {
            background: linear-gradient(135deg, #00ff9c 0%, #00dd88 100%);
            color: #000;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            font-size: 1em;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            display: inline-block;
            margin: 10px 5px;
        }

        .btn:hover {
            transform: scale(1.1);
            box-shadow: 0 0 30px rgba(0, 255, 156, 0.6);
        }

        .links-section {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>🔥 CUONGDEV | HACKER MODE 🔥</h1>
            <p class="tagline">Fullstack Developer | AI Engineer | Blockchain Enthusiast</p>
        </div>

        <div id="loading" class="loading">
            <div class="spinner"></div>
            <p>Loading GitHub data...</p>
        </div>

        <div id="content" style="display: none;">
            <div class="profile-section">
                <div class="profile-card">
                    <img id="avatar" class="avatar" src="" alt="Avatar">
                    <h2 class="profile-name" id="name"></h2>
                    <p id="username" style="color: #00dd88;"></p>
                    <p class="profile-bio" id="bio"></p>
                    <div class="profile-stats">
                        <div class="stat-box">
                            <div class="stat-number" id="repos">0</div>
                            <div class="stat-label">Repositories</div>
                        </div>
                        <div class="stat-box">
                            <div class="stat-number" id="followers">0</div>
                            <div class="stat-label">Followers</div>
                        </div>
                        <div class="stat-box">
                            <div class="stat-number" id="following">0</div>
                            <div class="stat-label">Following</div>
                        </div>
                    </div>
                    <div class="links-section">
                        <a id="profileLink" href="#" target="_blank" class="btn">View GitHub Profile</a>
                    </div>
                </div>

                <div class="info-card">
                    <h2>📍 Profile Information</h2>
                    <div class="info-item">
                        <strong>Location:</strong>
                        <span id="location">-</span>
                    </div>
                    <div class="info-item">
                        <strong>Company:</strong>
                        <span id="company">-</span>
                    </div>
                    <div class="info-item">
                        <strong>Blog:</strong>
                        <span id="blog">-</span>
                    </div>
                    <div class="info-item">
                        <strong>Email:</strong>
                        <span id="email">-</span>
                    </div>
                    <div class="info-item">
                        <strong>Twitter:</strong>
                        <span id="twitter">-</span>
                    </div>
                    <div class="info-item">
                        <strong>Created:</strong>
                        <span id="created">-</span>
                    </div>
                    <div class="info-item">
                        <strong>Updated:</strong>
                        <span id="updated">-</span>
                    </div>
                </div>
            </div>

            <h2 class="section-title">🚀 Featured Repositories</h2>
            <div id="repos" class="repos-grid"></div>
        </div>

        <div id="error" class="error" style="display: none;"></div>
    </div>

    <script>
        const username = 'chicuongdev2002';

        async function fetchGitHubData() {
            try {
                // Fetch user profile
                const userResponse = await fetch(`https://api.github.com/users/${username}`);
                if (!userResponse.ok) throw new Error('Failed to fetch user data');
                const userData = await userResponse.json();

                // Fetch repositories
                const reposResponse = await fetch(`https://api.github.com/users/${username}/repos?sort=updated&per_page=12`);
                if (!reposResponse.ok) throw new Error('Failed to fetch repositories');
                const reposData = await reposResponse.json();

                displayUserData(userData);
                displayRepos(reposData);

                document.getElementById('loading').style.display = 'none';
                document.getElementById('content').style.display = 'block';
            } catch (error) {
                console.error('Error:', error);
                document.getElementById('loading').style.display = 'none';
                document.getElementById('error').style.display = 'block';
                document.getElementById('error').textContent = `⚠️ Error: ${error.message}. Please check if the username is correct.`;
            }
        }

        function displayUserData(user) {
            document.getElementById('avatar').src = user.avatar_url;
            document.getElementById('name').textContent = user.name || user.login;
            document.getElementById('username').textContent = '@' + user.login;
            document.getElementById('bio').textContent = user.bio || 'No bio available';
            document.getElementById('repos').textContent = user.public_repos;
            document.getElementById('followers').textContent = user.followers;
            document.getElementById('following').textContent = user.following;
            document.getElementById('location').textContent = user.location || 'Not specified';
            document.getElementById('company').textContent = user.company || 'Not specified';
            document.getElementById('blog').innerHTML = user.blog ? `<a href="${user.blog}" target="_blank" style="color: #00ff9c;">${user.blog}</a>` : 'Not specified';
            document.getElementById('email').textContent = user.email || 'Not public';
            document.getElementById('twitter').textContent = user.twitter_username ? '@' + user.twitter_username : 'Not specified';
            document.getElementById('created').textContent = new Date(user.created_at).toLocaleDateString();
            document.getElementById('updated').textContent = new Date(user.updated_at).toLocaleDateString();
            document.getElementById('profileLink').href = user.html_url;
        }

        function displayRepos(repos) {
            const reposContainer = document.getElementById('repos');
            reposContainer.innerHTML = '';

            repos.forEach(repo => {
                const repoCard = document.createElement('div');
                repoCard.className = 'repo-card';
                repoCard.onclick = () => window.open(repo.html_url, '_blank');

                repoCard.innerHTML = `
                    <div class="repo-name">${repo.name}</div>
                    <div class="repo-description">${repo.description || 'No description available'}</div>
                    ${repo.language ? `<span class="language-tag">${repo.language}</span>` : ''}
                    <div class="repo-stats">
                        <div class="repo-stat">⭐ ${repo.stargazers_count}</div>
                        <div class="repo-stat">🔱 ${repo.forks_count}</div>
                        <div class="repo-stat">👁️ ${repo.watchers_count}</div>
                    </div>
                `;

                reposContainer.appendChild(repoCard);
            });
        }

        // Load data on page load
        fetchGitHubData();
    </script>
</body>
</html>
