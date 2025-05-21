
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
<script>
    // News API Configuration
    const API_KEY = '9185d55dbda14e73bfb4c1a08e85b429'; // Replace with your NewsAPI key
    const NEWS_API_URL = `https://newsapi.org/v2/top-headlines?country=us&apiKey=${API_KEY}`;
    
    // DOM Elements
    const featuredArticle = document.querySelector('.featured-article');
    const newsGrid = document.querySelector('.row.g-4');
    const navLinks = document.querySelectorAll('.nav-link');

    // Format date
    const formatDate = (dateString) => {
        const options = { year: 'numeric', month: 'long', day: 'numeric' };
        return new Date(dateString).toLocaleDateString(undefined, options);
    };

    // Create article card
    const createArticleCard = (article, category) => {
        return `
            <div class="col-md-6 col-lg-4">
                <div class="card article-card">
                    <img src="${article.urlToImage || 'https://source.unsplash.com/random/800x600?news'}" 
                         class="card-img-top" 
                         alt="${article.title}">
                    <div class="card-body">
                        <span class="category-badge">${category}</span>
                        <h5 class="mt-2">${article.title}</h5>
                        <p class="text-muted">${article.description?.substring(0, 100) || ''}...</p>
                        <div class="d-flex justify-content-between align-items-center">
                            <small>${formatDate(article.publishedAt)}</small>
                            <a href="${article.url}" target="_blank" class="btn btn-sm btn-outline-primary">Read More</a>
                        </div>
                    </div>
                </div>
            </div>
        `;
    };

    // Update featured article
    const updateFeaturedArticle = (article) => {
        featuredArticle.style.backgroundImage = `url('${article.urlToImage || 'https://source.unsplash.com/random/1200x800'}')`;
        featuredArticle.querySelector('h1').textContent = article.title;
        featuredArticle.querySelector('h5').textContent = article.author || 'Staff Writer';
    };

    // Fetch news articles
    const fetchNews = async (category = 'general') => {
        try {
            const response = await fetch(`https://newsapi.org/v2/top-headlines?country=us&category=${category}&apiKey=${API_KEY}`);
            const data = await response.json();
            
            if(data.articles.length === 0) throw new Error('No articles found');
            
            // Clear existing content
            newsGrid.innerHTML = '';
            
            // Update featured article with first result
            updateFeaturedArticle(data.articles[0]);
            
            // Create cards for other articles
            data.articles.slice(1).forEach(article => {
                if(article.title !== '[Removed]') { // Filter removed articles
                    newsGrid.innerHTML += createArticleCard(article, category);
                }
            });
            
        } catch (error) {
            console.error('Error fetching news:', error);
            newsGrid.innerHTML = `
                <div class="col-12 text-center py-5">
                    <h3>Unable to load news</h3>
                    <p>Please try again later</p>
                </div>
            `;
        }
    };

    // Category filter handler
    navLinks.forEach(link => {
        link.addEventListener('click', (e) => {
            e.preventDefault();
            const category = e.target.textContent.toLowerCase();
            navLinks.forEach(l => l.classList.remove('active'));
            e.target.classList.add('active');
            fetchNews(category);
        });
    });

    // Initial load
    document.addEventListener('DOMContentLoaded', () => fetchNews());
</script>


