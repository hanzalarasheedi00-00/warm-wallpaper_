# warm-wallpaper_
Warm Wallpaper — HD warm-colored wallpapers for phones and laptops, easy to view and download. for you and lovely wallpapers 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Warm Wallpapers</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f1eb;
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Landing Page Styles */
        .landing-page {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            position: relative;
            overflow: hidden;
        }
        
        .landing-content {
            text-align: center;
            color: white;
            z-index: 2;
            position: relative;
            max-width: 800px;
            padding: 40px;
            border-radius: 20px;
        }
        
        .landing-content h1 {
            font-size: 72px;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            background: linear-gradient(to right, #ff9966, #ff5e62);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 800;
            letter-spacing: 2px;
        }
        
        .landing-content p {
            font-size: 20px;
            margin-bottom: 30px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            color: #e6e6e6;
        }
        
        .btn {
            display: inline-block;
            background: linear-gradient(to right, #ff9966, #ff5e62);
            color: white;
            padding: 15px 40px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 18px;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.3);
        }
        
        .scene {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: 1;
        }
        
        .table {
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 600px;
            height: 300px;
            background: #0f3460;
            border-radius: 20px 20px 0 0;
            box-shadow: 0 -10px 30px rgba(0,0,0,0.3);
        }
        
        .person {
            position: absolute;
            bottom: 300px;
            left: 50%;
            transform: translateX(-50%);
            width: 200px;
            height: 300px;
        }
        
        .head {
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 80px;
            background: #FFDAB9;
            border-radius: 50%;
        }
        
        .body {
            position: absolute;
            top: 80px;
            left: 50%;
            transform: translateX(-50%);
            width: 120px;
            height: 150px;
            background: #1a1a2e;
            border-radius: 60px 60px 0 0;
        }
        
        .macbook {
            position: absolute;
            bottom: 320px;
            left: 50%;
            transform: translateX(-50%);
            width: 300px;
            height: 180px;
            background: #E8E8E8;
            border-radius: 10px 10px 0 0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }
        
        .screen {
            position: absolute;
            top: 10px;
            left: 10px;
            right: 10px;
            bottom: 40px;
            background: #1a1a1a;
            border-radius: 5px;
            overflow: hidden;
        }
        
        .screen-content {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: white;
            text-align: center;
        }
        
        .screen-content h3 {
            font-size: 18px;
            margin-bottom: 10px;
        }
        
        .keyboard {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 30px;
            background: #D3D3D3;
            border-radius: 0 0 10px 10px;
        }
        
        /* Main Website Styles (Hidden Initially) */
        .main-website {
            display: none;
        }
        
        /* Header Styles */
        header {
            background: linear-gradient(to right, #1a1a2e, #16213e);
            color: white;
            padding: 20px 0;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 28px;
            font-weight: 700;
            display: flex;
            align-items: center;
        }
        
        .logo i {
            margin-right: 10px;
            font-size: 32px;
            color: #ff9966;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 25px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 5px 10px;
            border-radius: 4px;
        }
        
        nav ul li a:hover {
            background-color: rgba(255,255,255,0.2);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1506905925346-21bda4d32df4?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 500px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            margin-bottom: 40px;
        }
        
        .hero-content {
            max-width: 800px;
            padding: 0 20px;
        }
        
        .hero-title {
            font-size: 82px;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            background: linear-gradient(to right, #ff9966, #ff5e62);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 800;
            letter-spacing: 3px;
        }
        
        .hero-subtitle {
            font-size: 24px;
            max-width: 700px;
            margin: 0 auto 30px;
            color: #e6e6e6;
        }
        
        /* Categories */
        .categories {
            margin-bottom: 50px;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            font-size: 32px;
            color: #1a1a2e;
            position: relative;
        }
        
        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: linear-gradient(to right, #ff9966, #ff5e62);
            margin: 10px auto;
            border-radius: 2px;
        }
        
        .category-list {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .category-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            width: 180px;
            text-align: center;
        }
        
        .category-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }
        
        .category-img {
            height: 120px;
            background-size: cover;
            background-position: center;
        }
        
        .category-name {
            padding: 15px;
            font-weight: 600;
            color: #333;
        }
        
        /* Wallpaper Gallery */
        .gallery {
            margin-bottom: 60px;
        }
        
        .gallery-filters {
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .filter-btn {
            background: white;
            border: 2px solid #ff5e62;
            color: #ff5e62;
            padding: 8px 20px;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 500;
        }
        
        .filter-btn.active, .filter-btn:hover {
            background: #ff5e62;
            color: white;
        }
        
        .wallpaper-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
        }
        
        .wallpaper-item {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            background: white;
        }
        
        .wallpaper-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }
        
        .wallpaper-img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            display: block;
        }
        
        .wallpaper-info {
            padding: 15px;
        }
        
        .wallpaper-title {
            font-weight: 600;
            margin-bottom: 5px;
            color: #333;
        }
        
        .wallpaper-resolution {
            color: #777;
            font-size: 14px;
            margin-bottom: 10px;
        }
        
        .download-btn {
            display: block;
            width: 100%;
            text-align: center;
            background: linear-gradient(to right, #ff9966, #ff5e62);
            color: white;
            padding: 8px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        .download-btn:hover {
            opacity: 0.9;
        }
        
        /* Admin Section */
        .admin-section {
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin-bottom: 60px;
            text-align: center;
            display: none;
        }
        
        .admin-section h2 {
            color: #1a1a2e;
            margin-bottom: 20px;
        }
        
        .upload-form {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: #555;
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }
        
        /* Footer */
        footer {
            background: #1a1a2e;
            color: white;
            padding: 40px 0 20px;
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-bottom: 30px;
        }
        
        .footer-column {
            flex: 1;
            min-width: 250px;
            margin-bottom: 30px;
        }
        
        .footer-column h3 {
            font-size: 20px;
            margin-bottom: 20px;
            color: #ff9966;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: #ddd;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .footer-column ul li a:hover {
            color: #ff9966;
            padding-left: 5px;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #2d2d42;
            color: #aaa;
            font-size: 14px;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
            }
            
            nav ul {
                margin-top: 20px;
            }
            
            .hero-title {
                font-size: 52px;
            }
            
            .hero-subtitle {
                font-size: 18px;
            }
            
            .wallpaper-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            }
            
            .table {
                width: 400px;
            }
            
            .macbook {
                width: 250px;
            }
            
            .landing-content h1 {
                font-size: 52px;
            }
        }
        
        @media (max-width: 480px) {
            .hero {
                height: 400px;
            }
            
            .hero-title {
                font-size: 42px;
            }
            
            .section-title {
                font-size: 26px;
            }
            
            .category-item {
                width: 140px;
            }
            
            .wallpaper-grid {
                grid-template-columns: 1fr;
            }
            
            .table {
                width: 300px;
            }
            
            .macbook {
                width: 200px;
                height: 150px;
            }
            
            .landing-content h1 {
                font-size: 42px;
            }
            
            .landing-content p {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>
    <!-- Landing Page -->
    <div class="landing-page" id="landingPage">
        <div class="scene">
            <div class="table"></div>
            <div class="person">
                <div class="head"></div>
                <div class="body"></div>
            </div>
            <div class="macbook">
                <div class="screen">
                    <div class="screen-content">
                        <h3>Warm Wallpapers</h3>
                        <p>Beautiful wallpapers for your devices</p>
                    </div>
                </div>
                <div class="keyboard"></div>
            </div>
        </div>
        <div class="landing-content">
            <h1>Warm Wallpapers</h1>
            <p>Discover a beautiful collection of warm-themed wallpapers to give your devices a cozy and inviting look.</p>
            <button class="btn" id="enterBtn">Explore Wallpapers</button>
        </div>
    </div>

    <!-- Main Website (Hidden Initially) -->
    <div class="main-website" id="mainWebsite">
        <!-- Header -->
        <header>
            <div class="container">
                <div class="header-content">
                    <div class="logo">
                        <i class="fas fa-fire"></i> Warm Wallpapers
                    </div>
                    <nav>
                        <ul>
                            <li><a href="#" class="nav-link" data-section="home">Home</a></li>
                            <li><a href="#" class="nav-link" data-section="gallery">Wallpapers</a></li>
                            <li><a href="#" class="nav-link" data-section="categories">Categories</a></li>
                            <li><a href="#" id="adminLink">Admin</a></li>
                        </ul>
                    </nav>
                </div>
            </div>
        </header>

        <!-- Hero Section -->
        <section class="hero" id="home">
            <div class="hero-content">
                <h1 class="hero-title">Warm Wallpapers</h1>
                <p class="hero-subtitle">Explore our collection of high-quality wallpapers to give your devices a warm and cozy look</p>
                <a href="#" class="btn nav-link" data-section="gallery">Browse Collection</a>
            </div>
        </section>

        <!-- Categories Section -->
        <section class="categories" id="categories">
            <div class="container">
                <h2 class="section-title">Categories</h2>
                <div class="category-list">
                    <div class="category-item">
                        <div class="category-img" style="background-image: url('https://images.unsplash.com/photo-1506905925346-21bda4d32df4?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                        <div class="category-name">Nature</div>
                    </div>
                    <div class="category-item">
                        <div class="category-img" style="background-image: url('https://images.unsplash.com/photo-1541701494587-cb58502866ab?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                        <div class="category-name">Abstract</div>
                    </div>
                    <div class="category-item">
                        <div class="category-img" style="background-image: url('https://images.unsplash.com/photo-1518837695005-2083093ee35b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                        <div class="category-name">Minimal</div>
                    </div>
                    <div class="category-item">
                        <div class="category-img" style="background-image: url('https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                        <div class="category-name">Patterns</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Wallpaper Gallery -->
        <section class="gallery" id="gallery">
            <div class="container">
                <h2 class="section-title">Featured Wallpapers</h2>
                <div class="gallery-filters">
                    <button class="filter-btn active">All</button>
                    <button class="filter-btn">Nature</button>
                    <button class="filter-btn">Abstract</button>
                    <button class="filter-btn">Minimal</button>
                </div>
                <div class="wallpaper-grid">
                    <!-- Wallpaper Item 1 -->
                    <div class="wallpaper-item">
                        <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Warm Mountain" class="wallpaper-img">
                        <div class="wallpaper-info">
                            <h3 class="wallpaper-title">Warm Mountain</h3>
                            <div class="wallpaper-resolution">1920x1080</div>
                            <a href="#" class="download-btn">Download</a>
                        </div>
                    </div>
                    
                    <!-- Wallpaper Item 2 -->
                    <div class="wallpaper-item">
                        <img src="https://images.unsplash.com/photo-1541701494587-cb58502866ab?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Golden Abstract" class="wallpaper-img">
                        <div class="wallpaper-info">
                            <h3 class="wallpaper-title">Golden Abstract</h3>
                            <div class="wallpaper-resolution">1920x1080</div>
                            <a href="#" class="download-btn">Download</a>
                        </div>
                    </div>
                    
                    <!-- Wallpaper Item 3 -->
                    <div class="wallpaper-item">
                        <img src="https://images.unsplash.com/photo-1518837695005-2083093ee35b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Minimal Warm" class="wallpaper-img">
                        <div class="wallpaper-info">
                            <h3 class="wallpaper-title">Minimal Warm</h3>
                            <div class="wallpaper-resolution">1920x1080</div>
                            <a href="#" class="download-btn">Download</a>
                        </div>
                    </div>
                    
                    <!-- Wallpaper Item 4 -->
                    <div class="wallpaper-item">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Warm Pattern" class="wallpaper-img">
                        <div class="wallpaper-info">
                            <h3 class="wallpaper-title">Warm Pattern</h3>
                            <div class="wallpaper-resolution">1920x1080</div>
                            <a href="#" class="download-btn">Download</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Admin Section (Hidden from regular users) -->
        <section class="admin-section" id="adminSection">
            <div class="container">
                <h2 class="section-title">Admin Panel</h2>
                <p>Welcome, Admin! You can upload new wallpapers here.</p>
                <form class="upload-form" id="uploadForm">
                    <div class="form-group">
                        <label for="wallpaper-title">Wallpaper Title</label>
                        <input type="text" id="wallpaper-title" class="form-control" placeholder="Enter wallpaper title" required>
                    </div>
                    <div class="form-group">
                        <label for="wallpaper-category">Category</label>
                        <select id="wallpaper-category" class="form-control" required>
                            <option value="">Select Category</option>
                            <option value="nature">Nature</option>
                            <option value="abstract">Abstract</option>
                            <option value="minimal">Minimal</option>
                            <option value="patterns">Patterns</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="wallpaper-file">Upload Wallpaper</label>
                        <input type="file" id="wallpaper-file" class="form-control" required>
                    </div>
                    <button type="submit" class="btn">Upload Wallpaper</button>
                </form>
            </div>
        </section>

        <!-- Footer -->
        <footer>
            <div class="container">
                <div class="footer-content">
                    <div class="footer-column">
                        <h3>Warm Wallpapers</h3>
                        <p>Your destination for beautiful, warm-themed wallpapers for all your devices.</p>
                    </div>
                    <div class="footer-column">
                        <h3>Quick Links</h3>
                        <ul>
                            <li><a href="#" class="nav-link" data-section="home">Home</a></li>
                            <li><a href="#" class="nav-link" data-section="gallery">Wallpapers</a></li>
                            <li><a href="#" class="nav-link" data-section="categories">Categories</a></li>
                        </ul>
                    </div>
                    <div class="footer-column">
                        <h3>Categories</h3>
                        <ul>
                            <li><a href="#">Nature</a></li>
                            <li><a href="#">Abstract</a></li>
                            <li><a href="#">Minimal</a></li>
                            <li><a href="#">Patterns</a></li>
                        </ul>
                    </div>
                </div>
                <div class="copyright">
                    &copy; 2023 Warm Wallpapers. All rights reserved.
                </div>
            </div>
        </footer>
    </div>

    <script>
        // Show main website when button is clicked
        document.getElementById('enterBtn').addEventListener('click', function() {
            document.getElementById('landingPage').style.display = 'none';
            document.getElementById('mainWebsite').style.display = 'block';
        });
        
        // Navigation functionality
        document.querySelectorAll('.nav-link').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const targetSection = this.getAttribute('data-section');
                
                // Scroll to the target section
                document.getElementById(targetSection).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Admin panel functionality
        document.getElementById('adminLink').addEventListener('click', function(e) {
            e.preventDefault();
            const password = prompt('Please enter admin password:');
            
            // In a real application, you would verify this on the server
            if (password === 'admin123') {
                document.getElementById('adminSection').style.display = 'block';
                document.getElementById('adminSection').scrollIntoView({
                    behavior: 'smooth'
                });
            } else {
                alert('Access denied. Incorrect password.');
            }
        });
        
        // Upload form submission
        document.getElementById('uploadForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Wallpaper uploaded successfully! It will be visible after approval.');
            this.reset();
        });
        
        // Filter functionality
        document.querySelectorAll('.filter-btn').forEach(button => {
            button.addEventListener('click', function() {
                // Remove active class from all buttons
                document.querySelectorAll('.filter-btn').forEach(btn => {
                    btn.classList.remove('active');
                });
                
                // Add active class to clicked button
                this.classList.add('active');
                
                // In a real implementation, you would filter the wallpapers here
                alert('Filtering by: ' + this.textContent);
            });
        });
    </script>
</body>
</html>
