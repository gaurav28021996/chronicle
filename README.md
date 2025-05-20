
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Daily Chronicle | Modern News Platform</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        :root {
            --primary-color: #2c3e50;
            --accent-color: #e74c3c;
            --text-color: #333;
            --light-bg: #f8f9fa;
        }

        body {
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
            color: var(--text-color);
            line-height: 1.6;
        }

        .navbar {
            background: var(--primary-color) !important;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .featured-article {
            height: 70vh;
            background-size: cover;
            background-position: center;
            position: relative;
            border-radius: 10px;
            overflow: hidden;
        }

        .featured-content {
            position: absolute;
            bottom: 0;
            background: linear-gradient(transparent, rgba(0,0,0,0.8));
            color: white;
            padding: 2rem;
            width: 100%;
        }

        .article-card {
            transition: transform 0.3s ease;
            border: none;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }

        .article-card:hover {
            transform: translateY(-5px);
        }

        .category-badge {
            background: var(--accent-color);
            color: white;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.9rem;
        }

        .newsletter-section {
            background: var(--light-bg);
            padding: 4rem 0;
        }

        .author-info {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin: 1.5rem 0;
        }

        .author-img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
        }

        @media (max-width: 768px) {
            .featured-article {
                height: 50vh;
            }
            
            .article-card {
                margin-bottom: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">The Daily Chronicle</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link active" href="#">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Politics</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Technology</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Business</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Culture</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Featured Article -->
    <div class="container mt-4">
        <div class="featured-article" style="background-image: url('https://source.unsplash.com/random/1200x800')">
            <div class="featured-content">
                <span class="category-badge">Featured Story</span>
                <h1 class="mt-2">Breaking: Major Climate Agreement Reached</h1>
                <div class="author-info">
                    <img src="https://source.unsplash.com/random/100x100?face" alt="Author" class="author-img">
                    <div>
                        <h5 class="mb-0">Sarah Johnson</h5>
                        <small>Senior Environmental Correspondent</small>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- News Grid -->
    <div class="container mt-5">
        <div class="row g-4">
            <div class="col-md-6 col-lg-4">
                <div class="card article-card">
                    <img src="https://source.unsplash.com/random/800x600?tech" class="card-img-top" alt="Tech News">
                    <div class="card-body">
                        <span class="category-badge">Technology</span>
                        <h5 class="mt-2">New AI Breakthrough Revolutionizes Healthcare</h5>
                        <p class="text-muted">Discover how machine learning is transforming medical diagnostics...</p>
                        <div class="d-flex justify-content-between align-items-center">
                            <small>15 Min Read</small>
                            <a href="#" class="btn btn-sm btn-outline-primary">Read More</a>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Repeat similar cards for other articles -->
            <div class="col-md-6 col-lg-4">
                <div class="card article-card">
                    <img src="https://source.unsplash.com/random/800x600?business" class="card-img-top" alt="Business News">
                    <div class="card-body">
                        <span class="category-badge">Business</span>
                        <h5 class="mt-2">Global Markets React to New Trade Policies</h5>
                        <p class="text-muted">Analysis of recent economic developments and market fluctuations...</p>
                        <div class="d-flex justify-content-between align-items-center">
                            <small>8 Min Read</small>
                            <a href="#" class="btn btn-sm btn-outline-primary">Read More</a>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col-md-6 col-lg-4">
                <div class="card article-card">
                    <img src="https://source.unsplash.com/random/800x600?culture" class="card-img-top" alt="Culture News">
                    <div class="card-body">
                        <span class="category-badge">Culture</span>
                        <h5 class="mt-2">Emerging Artists Redefine Modern Art Scene</h5>
                        <p class="text-muted">Exploring the latest trends in contemporary art exhibitions...</p>
                        <div class="d-flex justify-content-between align-items-center">
                            <small>12 Min Read</small>
                            <a href="#" class="btn btn-sm btn-outline-primary">Read More</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Newsletter Section -->
    <section class="newsletter-section mt-5">
        <div class="container text-center">
            <h2>Stay Informed</h2>
            <p class="lead">Subscribe to our daily newsletter for curated news updates</p>
            <div class="row justify-content-center">
                <div class="col-md-6">
                    <form class="input-group">
                        <input type="email" class="form-control" placeholder="Enter your email">
                        <button class="btn btn-primary" type="submit">Subscribe</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white mt-5 py-4">
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <h5>The Daily Chronicle</h5>
                    <p>Committed to delivering accurate, timely news</p>
                </div>
                <div class="col-md-3">
                    <h6>Categories</h6>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white">Politics</a></li>
                        <li><a href="#" class="text-white">Technology</a></li>
                        <li><a href="#" class="text-white">Business</a></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h6>Connect</h6>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white">Twitter</a></li>
                        <li><a href="#" class="text-white">Facebook</a></li>
                        <li><a href="#" class="text-white">Instagram</a></li>
                    </ul>
                </div>
            </div>
            <div class="text-center mt-3">
                <small>© 2024 The Daily Chronicle. All rights reserved. | <a href="#" class="text-white">Privacy Policy</a></small>
            </div>
        </div>
    </footer>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Admin Panel - The Daily Chronicle</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        :root {
            --primary-color: #2c3e50;
            --accent-color: #e74c3c;
            --light-bg: #f8f9fa;
        }

        .admin-sidebar {
            background: var(--primary-color);
            min-height: 100vh;
            color: white;
            padding: 20px;
        }

        .editor-toolbar {
            background: var(--light-bg);
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 15px;
        }

        #articleContent {
            min-height: 400px;
        }

        .article-preview {
            border: 1px solid #ddd;
            padding: 20px;
            margin-top: 20px;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="container-fluid">
        <div class="row">
            <!-- Sidebar -->
            <div class="col-md-3 col-lg-2 admin-sidebar">
                <h4>Admin Panel</h4>
                <ul class="nav flex-column">
                    <li class="nav-item">
                        <a class="nav-link text-white" href="#articles">Manage Articles</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-white" href="#new">New Article</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-white" href="#media">Media Library</a>
                    </li>
                </ul>
            </div>

            <!-- Main Content -->
            <div class="col-md-9 col-lg-10 p-4">
                <!-- Article Editor -->
                <div id="articleEditor">
                    <h3>Article Editor</h3>
                    <form id="articleForm">
                        <div class="mb-3">
                            <input type="text" class="form-control" id="articleTitle" placeholder="Article Title">
                        </div>
                        
                        <div class="row mb-3">
                            <div class="col-md-6">
                                <select class="form-select" id="articleCategory">
                                    <option value="politics">Politics</option>
                                    <option value="technology">Technology</option>
                                    <option value="business">Business</option>
                                    <option value="culture">Culture</option>
                                </select>
                            </div>
                            <div class="col-md-6">
                                <input type="text" class="form-control" id="articleImage" placeholder="Featured Image URL">
                            </div>
                        </div>

                        <div class="editor-toolbar">
                            <button type="button" class="btn btn-sm btn-outline-secondary" onclick="formatText('bold')"><strong>B</strong></button>
                            <button type="button" class="btn btn-sm btn-outline-secondary" onclick="formatText('italic')"><em>I</em></button>
                            <button type="button" class="btn btn-sm btn-outline-secondary" onclick="insertHeading()">H2</button>
                        </div>

                        <div class="mb-3">
                            <textarea class="form-control" id="articleContent" placeholder="Write your article here..."></textarea>
                        </div>

                        <div class="article-preview">
                            <h5>Preview</h5>
                            <div id="livePreview"></div>
                        </div>

                        <div class="mt-3">
                            <button type="submit" class="btn btn-primary">Publish Article</button>
                            <button type="button" class="btn btn-secondary" onclick="saveDraft()">Save Draft</button>
                        </div>
                    </form>
                </div>

                <!-- Articles List -->
                <div id="articlesList" class="mt-5">
                    <h4>Existing Articles</h4>
                    <div class="list-group" id="articlesContainer">
                        <!-- Articles will be loaded here -->
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

    <!-- Admin Script -->
    <script>
        // Temporary storage (Replace with real database in production)
        let articles = JSON.parse(localStorage.getItem('articles')) || [];

        // Initialize
        document.addEventListener('DOMContentLoaded', () => {
            loadArticles();
            setupPreview();
        });

        // Form submission
        document.getElementById('articleForm').addEventListener('submit', (e) => {
            e.preventDefault();
            saveArticle();
        });

        function saveArticle() {
            const article = {
                id: Date.now(),
                title: document.getElementById('articleTitle').value,
                category: document.getElementById('articleCategory').value,
                content: document.getElementById('articleContent').value,
                image: document.getElementById('articleImage').value,
                author: "Admin",
                date: new Date().toISOString()
            };

            articles.push(article);
            localStorage.setItem('articles', JSON.stringify(articles));
            loadArticles();
            resetForm();
        }

        function loadArticles() {
            const container = document.getElementById('articlesContainer');
            container.innerHTML = articles.map(article => `
                <div class="list-group-item">
                    <div class="d-flex justify-content-between align-items-center">
                        <div>
                            <h5>${article.title}</h5>
                            <small>${new Date(article.date).toLocaleDateString()} - ${article.category}</small>
                        </div>
                        <div>
                            <button class="btn btn-sm btn-warning" onclick="editArticle(${article.id})">Edit</button>
                            <button class="btn btn-sm btn-danger" onclick="deleteArticle(${article.id})">Delete</button>
                        </div>
                    </div>
                </div>
            `).join('');
        }

        function editArticle(id) {
            const article = articles.find(a => a.id === id);
            if (article) {
                document.getElementById('articleTitle').value = article.title;
                document.getElementById('articleCategory').value = article.category;
                document.getElementById('articleContent').value = article.content;
                document.getElementById('articleImage').value = article.image;
            }
        }

        function deleteArticle(id) {
            if (confirm('Are you sure you want to delete this article?')) {
                articles = articles.filter(a => a.id !== id);
                localStorage.setItem('articles', JSON.stringify(articles));
                loadArticles();
            }
        }

        function resetForm() {
            document.getElementById('articleForm').reset();
            document.getElementById('livePreview').innerHTML = '';
        }

        function setupPreview() {
            const contentField = document.getElementById('articleContent');
            contentField.addEventListener('input', () => {
                document.getElementById('livePreview').innerHTML = 
                    contentField.value.replace(/\n/g, '<br>');
            });
        }

        // Basic text formatting
        function formatText(type) {
            const textarea = document.getElementById('articleContent');
            const start = textarea.selectionStart;
            const end = textarea.selectionEnd;
            const selectedText = textarea.value.substring(start, end);
            
            const formats = {
                bold: [`**${selectedText}**`, '**'],
                italic: [`*${selectedText}*`, '*']
            };

            if (formats[type]) {
                textarea.value = textarea.value.substring(0, start) + 
                               formats[type][0] + 
                               textarea.value.substring(end);
                textarea.focus();
                textarea.selectionStart = start + formats[type][1].length;
                textarea.selectionEnd = end + formats[type][1].length;
            }
        }

        function insertHeading() {
            const textarea = document.getElementById('articleContent');
            const start = textarea.selectionStart;
            textarea.value = textarea.value.substring(0, start) + 
                            '## Heading\n' + 
                            textarea.value.substring(start);
            textarea.focus();
        }

        function saveDraft() {
            const draft = {
                title: document.getElementById('articleTitle').value,
                content: document.getElementById('articleContent').value,
                date: new Date()
            };
            localStorage.setItem('draft', JSON.stringify(draft));
            alert('Draft saved successfully');
        }
    </script>
</body>
</html>    

<!-- Add at top of <body> -->
<div id="loginOverlay" style="position: fixed; top:0; left:0; width:100%; height:100%; background: white; z-index: 9999;">
    <div class="container" style="max-width: 400px; margin-top: 100px;">
        <h3>Admin Login</h3>
        <input type="password" id="adminPassword" class="form-control mb-3" placeholder="Enter Admin Password">
        <button onclick="checkPassword()" class="btn btn-primary">Login</button>
    </div>
</div>

<script>
// Simple password protection
function checkPassword() {
    if (document.getElementById('adminPassword').value === 'your_password') {
        document.getElementById('loginOverlay').style.display = 'none';
    } else {
        alert('Incorrect password');
    }
}
</script>
