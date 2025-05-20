
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


<!DOCTYPE html>
<html lang="en" data-bs-theme="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced Admin Panel - The Daily Chronicle</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdn.quilljs.com/1.3.7/quill.snow.css" rel="stylesheet">
    <style>
        :root {
            --primary-color: #2c3e50;
            --accent-color: #e74c3c;
            --sidebar-width: 280px;
        }

        .admin-sidebar {
            background: var(--primary-color);
            width: var(--sidebar-width);
            height: 100vh;
            position: fixed;
            padding: 20px;
            transition: transform 0.3s;
            z-index: 1000;
        }

        .main-content {
            margin-left: var(--sidebar-width);
            padding: 30px;
            min-height: 100vh;
        }

        .ql-toolbar {
            border-radius: 8px 8px 0 0;
        }

        .ql-container {
            border-radius: 0 0 8px 8px;
            min-height: 400px;
        }

        .media-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 15px;
        }

        .media-item {
            position: relative;
            cursor: pointer;
            transition: transform 0.2s;
        }

        .media-item:hover {
            transform: scale(1.05);
        }

        @media (max-width: 768px) {
            .admin-sidebar {
                transform: translateX(-100%);
            }
            .main-content {
                margin-left: 0;
            }
            .sidebar-toggle {
                display: block !important;
            }
        }
    </style>
</head>
<body>
    <!-- Sidebar Toggle -->
    <button class="sidebar-toggle btn btn-primary position-fixed d-none" 
            style="z-index: 999; top: 10px; left: 10px;"
            onclick="toggleSidebar()">
        ☰
    </button>

    <!-- Sidebar -->
    <nav class="admin-sidebar text-white">
        <div class="d-flex flex-column h-100">
            <h4 class="mb-4">News Dashboard</h4>
            
            <div class="nav flex-column flex-grow-1">
                <div class="nav-item mb-3">
                    <button class="btn btn-dark w-100 text-start" 
                            onclick="showSection('editor')">
                        ✍️ Article Editor
                    </button>
                </div>
                <div class="nav-item mb-3">
                    <button class="btn btn-dark w-100 text-start"
                            onclick="showSection('media')">
                        🖼️ Media Library
                    </button>
                </div>
                <div class="nav-item mb-3">
                    <button class="btn btn-dark w-100 text-start"
                            onclick="showSection('categories')">
                        🏷️ Categories
                    </button>
                </div>
                <div class="nav-item mb-3">
                    <button class="btn btn-dark w-100 text-start"
                            onclick="showSection('analytics')">
                        📈 Analytics
                    </button>
                </div>
            </div>

            <div class="mt-auto">
                <div class="dropdown">
                    <button class="btn btn-secondary w-100 dropdown-toggle" 
                            type="button" data-bs-toggle="dropdown">
                        ⚙️ Settings
                    </button>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#" onclick="toggleTheme()">🎨 Toggle Theme</a></li>
                        <li><a class="dropdown-item" href="#" data-bs-toggle="modal" 
                               data-bs-target="#pluginsModal">🔌 Plugins</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="main-content bg-body-tertiary">
        <!-- Article Editor Section -->
        <section id="editorSection" class="section-content">
            <div class="card shadow-lg">
                <div class="card-body">
                    <h3 class="mb-4">📝 Article Editor</h3>
                    <form id="articleForm">
                        <div class="row g-3 mb-4">
                            <div class="col-md-8">
                                <input type="text" class="form-control form-control-lg" 
                                       id="articleTitle" placeholder="Article Title">
                            </div>
                            <div class="col-md-4">
                                <select class="form-select" id="articleStatus">
                                    <option value="draft">Draft</option>
                                    <option value="published">Publish Now</option>
                                    <option value="scheduled">Schedule</option>
                                </select>
                            </div>
                        </div>

                        <div class="row g-3 mb-4">
                            <div class="col-md-6">
                                <select class="form-select" id="articleCategory" multiple>
                                    <!-- Categories loaded dynamically -->
                                </select>
                            </div>
                            <div class="col-md-6">
                                <input type="text" class="form-control" 
                                       id="featuredImage" placeholder="Featured Image URL">
                            </div>
                        </div>

                        <!-- Rich Text Editor -->
                        <div id="editor" style="height: 500px;"></div>

                        <!-- SEO Plugin -->
                        <div class="card mt-4">
                            <div class="card-header">🔍 SEO Optimizer</div>
                            <div class="card-body">
                                <div class="mb-3">
                                    <label>Meta Description</label>
                                    <textarea class="form-control" id="metaDescription" 
                                              rows="3"></textarea>
                                </div>
                                <div class="mb-3">
                                    <label>Slug</label>
                                    <input type="text" class="form-control" id="articleSlug">
                                </div>
                            </div>
                        </div>

                        <div class="mt-4 d-flex gap-2">
                            <button type="submit" class="btn btn-primary px-4">
                                💾 Save Article
                            </button>
                            <button type="button" class="btn btn-outline-secondary"
                                    onclick="showPreview()">
                                👁️ Preview
                            </button>
                        </div>
                    </form>
                </div>
            </div>
        </section>

        <!-- Media Library Section -->
        <section id="mediaSection" class="section-content d-none">
            <div class="card shadow-lg">
                <div class="card-body">
                    <h3 class="mb-4">🖼️ Media Library</h3>
                    <div class="mb-4">
                        <input type="file" class="form-control" id="mediaUpload" 
                               accept="image/*" multiple>
                    </div>
                    <div class="media-gallery" id="mediaGallery">
                        <!-- Media items loaded dynamically -->
                    </div>
                </div>
            </div>
        </section>

        <!-- Plugins Modal -->
        <div class="modal fade" id="pluginsModal">
            <div class="modal-dialog modal-lg">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title">🔌 Available Plugins</h5>
                        <button type="button" class="btn-close" 
                                data-bs-dismiss="modal"></button>
                    </div>
                    <div class="modal-body">
                        <div class="row g-3">
                            <div class="col-md-6">
                                <div class="card">
                                    <div class="card-body">
                                        <h5>SEO Toolkit</h5>
                                        <p>Advanced SEO analysis and optimization</p>
                                        <button class="btn btn-sm btn-success">Activate</button>
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-6">
                                <div class="card">
                                    <div class="card-body">
                                        <h5>Social Auto-Share</h5>
                                        <p>Automatically share articles on social media</p>
                                        <button class="btn btn-sm btn-success">Activate</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- Scripts -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdn.quilljs.com/1.3.7/quill.js"></script>
    <script>
        // Initialize Quill Editor
        const quill = new Quill('#editor', {
            theme: 'snow',
            modules: {
                toolbar: [
                    ['bold', 'italic', 'underline', 'strike'],
                    ['blockquote', 'code-block'],
                    [{ 'header': 1 }, { 'header': 2 }],
                    [{ 'list': 'ordered'}, { 'list': 'bullet' }],
                    ['link', 'image', 'video'],
                    ['clean']
                ]
            }
        });

        // Admin Panel Functionality
        let currentTheme = 'dark';
        let activeSection = 'editor';

        function toggleSidebar() {
            document.querySelector('.admin-sidebar').style.transform = 
                document.querySelector('.admin-sidebar').style.transform === 'translateX(0px)' ?
                'translateX(-100%)' : 'translateX(0px)';
        }

        function showSection(sectionId) {
            document.querySelectorAll('.section-content').forEach(el => 
                el.classList.add('d-none'));
            document.getElementById(`${sectionId}Section`).classList.remove('d-none');
            activeSection = sectionId;
        }

        function toggleTheme() {
            currentTheme = currentTheme === 'dark' ? 'light' : 'dark';
            document.documentElement.setAttribute('data-bs-theme', currentTheme);
            localStorage.setItem('adminTheme', currentTheme);
        }

        // Initialize theme
        const savedTheme = localStorage.getItem('adminTheme') || 'dark';
        document.documentElement.setAttribute('data-bs-theme', savedTheme);
        currentTheme = savedTheme;

        // Media Upload Handling
        document.getElementById('mediaUpload').addEventListener('change', function(e) {
            Array.from(e.target.files).forEach(file => {
                const reader = new FileReader();
                reader.onload = (event) => {
                    const mediaItem = document.createElement('div');
                    mediaItem.className = 'media-item';
                    mediaItem.innerHTML = `
                        <img src="${event.target.result}" 
                             class="img-fluid rounded" 
                             alt="Upload">
                    `;
                    document.getElementById('mediaGallery').appendChild(mediaItem);
                };
                reader.readAsDataURL(file);
            });
        });

        // Category Management
        let categories = JSON.parse(localStorage.getItem('categories')) || [
            'Technology', 'Politics', 'Business', 'Culture'
        ];

        function updateCategorySelect() {
            const select = document.getElementById('articleCategory');
            select.innerHTML = categories.map(cat => `
                <option value="${cat}">${cat}</option>
            `).join('');
        }
        updateCategorySelect();

        // Article Saving
        document.getElementById('articleForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const article = {
                id: Date.now(),
                title: document.getElementById('articleTitle').value,
                content: quill.root.innerHTML,
                categories: Array.from(document.getElementById('articleCategory').selectedOptions)
                                .map(opt => opt.value),
                metaDescription: document.getElementById('metaDescription').value,
                slug: document.getElementById('articleSlug').value,
                status: document.getElementById('articleStatus').value,
                featuredImage: document.getElementById('featuredImage').value,
                timestamp: new Date().toISOString()
            };

            const articles = JSON.parse(localStorage.getItem('articles')) || [];
            articles.push(article);
            localStorage.setItem('articles', JSON.stringify(articles));

            alert('Article saved successfully!');
        });

        // Responsive Adjustments
        window.addEventListener('resize', () => {
            if (window.innerWidth > 768) {
                document.querySelector('.admin-sidebar').style.transform = 'translateX(0)';
            }
        });
    </script>


</body>
</html>

