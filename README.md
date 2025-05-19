# bestrestosite
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Hyderabad Food Guide - Discover the best restaurants, biryani spots, and street food in Hyderabad with detailed reviews and ratings">
    <meta name="keywords" content="Hyderabad food, best biryani Hyderabad, Paradise restaurant, street food Hyderabad, food blog India">
    <meta name="author" content="Hyderabad Food Explorer">
    <meta property="og:title" content="Hyderabad Food Guide | Best Restaurants & Street Food">
    <meta property="og:description" content="Discover the best culinary experiences in Hyderabad with our expert reviews">
    <meta property="og:image" content="https://example.com/hyderabad-food-banner.jpg">
    <meta property="og:url" content="https://example.com">
    <meta name="twitter:card" content="summary_large_image">
    <title>Hyderabad Food Guide | Best Restaurants & Street Food</title>
    <style>
        /* Base Styles */
        :root {
            --primary-color: #e67e22;
            --secondary-color: #d35400;
            --dark-color: #333;
            --light-color: #f4f4f4;
            --text-color: #555;
            --white: #fff;
            --black: #000;
            --box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--white);
            overflow-x: hidden;
        }

        h1, h2, h3, h4 {
            font-family: 'Playfair Display', serif;
            color: var(--dark-color);
            line-height: 1.2;
        }

        a {
            text-decoration: none;
            color: var(--primary-color);
            transition: var(--transition);
        }

        a:hover {
            color: var(--secondary-color);
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        ul {
            list-style: none;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .btn {
            display: inline-block;
            background: var(--primary-color);
            color: var(--white);
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 600;
        }

        .btn:hover {
            background: var(--secondary-color);
            transform: translateY(-3px);
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
            font-size: 2.5rem;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--primary-color);
            margin: 15px auto;
        }

        /* Header Styles */
        .header {
            background-color: var(--white);
            box-shadow: var(--box-shadow);
            position: fixed;
            width: 100%;
            top: 0;
            left: 0;
            z-index: 1000;
            padding: 15px 0;
        }

        .header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo h1 {
            font-size: 1.8rem;
            color: var(--primary-color);
            margin-bottom: 5px;
        }

        .logo p {
            font-size: 0.8rem;
            color: var(--text-color);
        }

        .main-nav ul {
            display: flex;
        }

        .main-nav ul li {
            margin-left: 30px;
        }

        .main-nav ul li a {
            color: var(--dark-color);
            font-weight: 600;
            position: relative;
        }

        .main-nav ul li a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary-color);
            transition: var(--transition);
        }

        .main-nav ul li a:hover::after,
        .main-nav ul li a.active::after {
            width: 100%;
        }

        .main-nav ul li a.active {
            color: var(--primary-color);
        }

        .mobile-menu-btn {
            display: none;
            cursor: pointer;
        }

        .mobile-menu-btn span {
            display: block;
            width: 25px;
            height: 3px;
            background: var(--dark-color);
            margin: 5px 0;
            transition: var(--transition);
        }

        /* Ad Banner Styles */
        .ad-banner {
            background: var(--light-color);
            padding: 15px 0;
            margin-top: 80px;
        }

        .ad-unit {
            padding: 30px 0;
            background: var(--light-color);
        }

        /* Main Content Styles */
        .main-content {
            padding: 40px 0;
        }

        /* Featured Section */
        .featured-section {
            padding: 60px 0;
        }

        .featured-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .featured-card {
            background: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
        }

        .featured-card:hover {
            transform: translateY(-10px);
        }

        .featured-img {
            height: 200px;
            overflow: hidden;
        }

        .featured-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .featured-card:hover .featured-img img {
            transform: scale(1.1);
        }

        .featured-content {
            padding: 20px;
        }

        .featured-content h3 {
            margin-bottom: 10px;
            font-size: 1.5rem;
        }

        .featured-content p {
            margin-bottom: 15px;
            color: var(--text-color);
        }

        .featured-rating {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }

        .featured-rating .stars {
            color: #f1c40f;
            margin-right: 10px;
        }

        .featured-meta {
            display: flex;
            justify-content: space-between;
            font-size: 0.9rem;
            color: #777;
        }

        /* Restaurants Section */
        .restaurants-section {
            padding: 60px 0;
        }

        .filter-options {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: 30px;
            gap: 10px;
        }

        .filter-btn {
            padding: 8px 20px;
            background: var(--light-color);
            color: var(--dark-color);
            border: none;
            border-radius: 30px;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 500;
        }

        .filter-btn.active,
        .filter-btn:hover {
            background: var(--primary-color);
            color: var(--white);
        }

        .restaurants-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .restaurant-card {
            background: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
        }

        .restaurant-card:hover {
            transform: translateY(-5px);
        }

        .restaurant-img {
            height: 180px;
            overflow: hidden;
            position: relative;
        }

        .restaurant-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .restaurant-tag {
            position: absolute;
            top: 15px;
            right: 15px;
            background: var(--primary-color);
            color: var(--white);
            padding: 5px 10px;
            border-radius: 5px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .restaurant-content {
            padding: 20px;
        }

        .restaurant-content h3 {
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .restaurant-location {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
            color: #777;
            font-size: 0.9rem;
        }

        .restaurant-location i {
            margin-right: 5px;
        }

        .restaurant-desc {
            margin-bottom: 15px;
            font-size: 0.9rem;
            display: -webkit-box;
            -webkit-line-clamp: 3;
            -webkit-box-orient: vertical;
            overflow: hidden;
        }

        .restaurant-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 15px;
            border-top: 1px solid #eee;
        }

        .restaurant-rating {
            display: flex;
            align-items: center;
        }

        .restaurant-rating .stars {
            color: #f1c40f;
            margin-right: 5px;
        }

        .restaurant-price {
            font-weight: 600;
            color: var(--dark-color);
        }

        /* Street Food Section */
        .street-food-section {
            padding: 60px 0;
        }

        .street-food-map {
            height: 400px;
            background: #eee;
            margin-bottom: 40px;
            border-radius: 10px;
            overflow: hidden;
            position: relative;
        }

        .street-food-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .street-food-item {
            background: var(--white);
            padding: 20px;
            border-radius: 10px;
            box-shadow: var(--box-shadow);
            display: flex;
            align-items: center;
            transition: var(--transition);
        }

        .street-food-item:hover {
            transform: translateY(-5px);
        }

        .street-food-icon {
            width: 60px;
            height: 60px;
            background: var(--primary-color);
            color: var(--white);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            margin-right: 15px;
            flex-shrink: 0;
        }

        .street-food-content h4 {
            margin-bottom: 5px;
        }

        .street-food-content p {
            font-size: 0.9rem;
            color: #777;
        }

        /* Biryani Section */
        .biryani-section {
            padding: 60px 0;
            background: url('biryani-bg.jpg') no-repeat center center/cover;
            position: relative;
            color: var(--white);
        }

        .biryani-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
        }

        .biryani-section .container {
            position: relative;
            z-index: 1;
        }

        .biryani-section .section-title {
            color: var(--white);
        }

        .biryani-section .section-title::after {
            background: var(--white);
        }

        .biryani-guide {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .biryani-card {
            background: rgba(255, 255, 255, 0.9);
            padding: 25px;
            border-radius: 10px;
            color: var(--dark-color);
            transition: var(--transition);
        }

        .biryani-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }

        .biryani-card h3 {
            color: var(--primary-color);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }

        .biryani-card p {
            margin-bottom: 15px;
        }

        .biryani-specs {
            display: flex;
            margin-bottom: 15px;
        }

        .biryani-spec {
            margin-right: 20px;
        }

        .biryani-spec i {
            color: var(--primary-color);
            margin-right: 5px;
        }

        .biryani-price {
            font-size: 1.2rem;
            font-weight: 700;
            color: var(--secondary-color);
        }

        /* Testimonials Section */
        .testimonials-section {
            padding: 60px 0;
            background: var(--light-color);
        }

        .testimonials-slider {
            display: flex;
            overflow-x: auto;
            scroll-snap-type: x mandatory;
            gap: 30px;
            padding: 20px 0;
            margin-bottom: 40px;
            -webkit-overflow-scrolling: touch;
        }

        .testimonial-card {
            min-width: 300px;
            scroll-snap-align: start;
            background: var(--white);
            padding: 25px;
            border-radius: 10px;
            box-shadow: var(--box-shadow);
        }

        .testimonial-header {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }

        .testimonial-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            overflow: hidden;
            margin-right: 15px;
        }

        .testimonial-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .testimonial-user h4 {
            margin-bottom: 5px;
        }

        .testimonial-rating {
            color: #f1c40f;
            font-size: 0.9rem;
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 15px;
        }

        .testimonial-restaurant {
            font-size: 0.9rem;
            color: #777;
        }

        .testimonial-restaurant a {
            color: var(--primary-color);
        }

        .add-testimonial {
            background: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: var(--box-shadow);
            max-width: 600px;
            margin: 0 auto;
        }

        .add-testimonial h3 {
            text-align: center;
            margin-bottom: 20px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: 'Poppins', sans-serif;
            transition: var(--transition);
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--primary-color);
        }

        .form-group textarea {
            min-height: 120px;
            resize: vertical;
        }

        .star-rating {
            display: inline-block;
            margin-left: 10px;
        }

        .star {
            font-size: 1.5rem;
            color: #ddd;
            cursor: pointer;
            transition: var(--transition);
        }

        .star:hover,
        .star.active {
            color: #f1c40f;
        }

        .submit-btn {
            width: 100%;
            padding: 12px;
            font-size: 1rem;
        }

        /* About Section */
        .about-section {
            padding: 60px 0;
        }

        .about-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .about-content p {
            margin-bottom: 20px;
        }

        /* Newsletter Section */
        .newsletter-section {
            padding: 60px 0;
            background: var(--primary-color);
            color: var(--white);
            text-align: center;
        }

        .newsletter-section h2 {
            color: var(--white);
            margin-bottom: 20px;
        }

        .newsletter-section p {
            max-width: 600px;
            margin: 0 auto 30px;
        }

        #newsletterForm {
            display: flex;
            max-width: 500px;
            margin: 0 auto;
        }

        #newsletterForm input {
            flex: 1;
            padding: 12px 15px;
            border: none;
            border-radius: 5px 0 0 5px;
            font-family: 'Poppins', sans-serif;
        }

        #newsletterForm button {
            padding: 12px 20px;
            background: var(--dark-color);
            color: var(--white);
            border: none;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 600;
        }

        #newsletterForm button:hover {
            background: #222;
        }

        /* Footer Styles */
        .footer {
            background: var(--dark-color);
            color: var(--white);
            padding: 60px 0 0;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-col h3 {
            color: var(--white);
            margin-bottom: 20px;
            font-size: 1.3rem;
        }

        .footer-col p {
            margin-bottom: 15px;
            opacity: 0.8;
        }

        .footer-col ul li {
            margin-bottom: 10px;
        }

        .footer-col ul li a {
            color: #bbb;
            transition: var(--transition);
        }

        .footer-col ul li a:hover {
            color: var(--primary-color);
            padding-left: 5px;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: var(--white);
            transition: var(--transition);
        }

        .social-links a:hover {
            background: var(--primary-color);
            transform: translateY(-3px);
        }

        .footer-bottom {
            padding: 20px 0;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            text-align: center;
            font-size: 0.9rem;
            opacity: 0.7;
        }

        .footer-bottom ul {
            display: flex;
            justify-content: center;
            margin-top: 15px;
        }

        .footer-bottom ul li {
            margin: 0 10px;
        }

        .footer-bottom ul li a {
            color: #bbb;
        }

        /* Responsive Styles */
        @media (max-width: 992px) {
            .section-title {
                font-size: 2rem;
            }
            
            .featured-grid {
                grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            }
        }

        @media (max-width: 768px) {
            .mobile-menu-btn {
                display: block;
            }
            
            .main-nav {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 80px);
                background: var(--white);
                transition: var(--transition);
                padding: 30px 0;
                overflow-y: auto;
            }
            
            .main-nav.active {
                left: 0;
            }
            
            .main-nav ul {
                flex-direction: column;
            }
            
            .main-nav ul li {
                margin: 15px 0;
                text-align: center;
            }
            
            .mobile-menu-btn.active span:nth-child(1) {
                transform: rotate(45deg) translate(5px, 5px);
            }
            
            .mobile-menu-btn.active span:nth-child(2) {
                opacity: 0;
            }
            
            .mobile-menu-btn.active span:nth-child(3) {
                transform: rotate(-45deg) translate(7px, -6px);
            }
            
            .ad-banner {
                margin-top: 70px;
            }
            
            #newsletterForm {
                flex-direction: column;
            }
            
            #newsletterForm input {
                border-radius: 5px;
                margin-bottom: 10px;
            }
            
            #newsletterForm button {
                border-radius: 5px;
                width: 100%;
            }
        }

        @media (max-width: 576px) {
            .section-title {
                font-size: 1.8rem;
            }
            
            .filter-options {
                justify-content: flex-start;
            }
            
            .restaurants-grid {
                grid-template-columns: 1fr;
            }
            
            .featured-grid {
                grid-template-columns: 1fr;
            }
            
            .footer-grid {
                grid-template-columns: 1fr;
            }
            
            .footer-bottom ul {
                flex-direction: column;
            }
            
            .footer-bottom ul li {
                margin: 5px 0;
            }
        }
    </style>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX" crossorigin="anonymous"></script>
</head>
<body>
    <header class="header">
        <div class="container">
            <div class="logo">
                <h1>Hyderabad Food Guide</h1>
                <p>Discover the City of Nizams' Culinary Treasures</p>
            </div>
            <nav class="main-nav">
                <ul>
                    <li><a href="#home" class="active">Home</a></li>
                    <li><a href="#restaurants">Restaurants</a></li>
                    <li><a href="#street-food">Street Food</a></li>
                    <li><a href="#biryani-trail">Biryani Trail</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
            <div class="mobile-menu-btn">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </div>
    </header>

    <div class="ad-banner">
        <div class="container">
            <!-- Google AdSense Banner Ad -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                 data-ad-slot="XXXXXXXXXX"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>
    </div>

    <main class="main-content">
        <section id="featured" class="featured-section">
            <div class="container">
                <h2>Featured Hyderabad Eateries</h2>
                <div class="featured-grid" id="featuredRestaurants">
                    <!-- Dynamically loaded from JavaScript -->
                </div>
            </div>
        </section>

        <div class="ad-unit">
            <div class="container">
                <!-- Google AdSense Rectangle Ad -->
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                     data-ad-slot="XXXXXXXXXX"
                     data-ad-format="rectangle"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
        </div>

        <section id="restaurants" class="restaurants-section">
            <div class="container">
                <h2>Best Restaurants in Hyderabad</h2>
                <div class="filter-options">
                    <button class="filter-btn active" data-filter="all">All</button>
                    <button class="filter-btn" data-filter="biryani">Biryani</button>
                    <button class="filter-btn" data-filter="fine-dining">Fine Dining</button>
                    <button class="filter-btn" data-filter="cafe">Cafés</button>
                    <button class="filter-btn" data-filter="vegetarian">Vegetarian</button>
                </div>
                <div class="restaurants-grid" id="restaurantsGrid">
                    <!-- Dynamically loaded from JavaScript -->
                </div>
            </div>
        </section>

        <section id="street-food" class="street-food-section">
            <div class="container">
                <h2>Hyderabad Street Food Hotspots</h2>
                <div class="street-food-map" id="streetFoodMap">
                    <!-- Map integration would go here -->
                    <img src="https://maps.googleapis.com/maps/api/staticmap?center=Hyderabad,India&zoom=12&size=800x400&maptype=roadmap&markers=color:red%7C17.3850,78.4867&key=YOUR_API_KEY" alt="Hyderabad Street Food Map" style="width:100%;height:100%;object-fit:cover;">
                </div>
                <div class="street-food-list" id="streetFoodList">
                    <!-- Dynamically loaded from JavaScript -->
                </div>
            </div>
        </section>

        <section id="biryani-trail" class="biryani-section">
            <div class="container">
                <h2>Hyderabad's Legendary Biryani Trail</h2>
                <div class="biryani-guide" id="biryaniGuide">
                    <!-- Dynamically loaded from JavaScript -->
                </div>
            </div>
        </section>

        <section class="testimonials-section">
            <div class="container">
                <h2>Foodie Testimonials</h2>
                <div class="testimonials-slider" id="testimonialsSlider">
                    <!-- Dynamically loaded from JavaScript -->
                </div>
                <div class="add-testimonial">
                    <h3>Share Your Experience</h3>
                    <form id="testimonialForm">
                        <div class="form-group">
                            <input type="text" id="userName" placeholder="Your Name" required>
                        </div>
                        <div class="form-group">
                            <input type="email" id="userEmail" placeholder="Your Email">
                        </div>
                        <div class="form-group">
                            <textarea id="userTestimonial" placeholder="Your food experience in Hyderabad..." required></textarea>
                        </div>
                        <div class="form-group">
                            <select id="restaurantVisited">
                                <option value="">Select Restaurant (optional)</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="userRating">Your Rating:</label>
                            <div class="star-rating">
                                <span class="star" data-value="1">★</span>
                                <span class="star" data-value="2">★</span>
                                <span class="star" data-value="3">★</span>
                                <span class="star" data-value="4">★</span>
                                <span class="star" data-value="5">★</span>
                            </div>
                            <input type="hidden" id="userRating" value="0">
                        </div>
                        <button type="submit" class="submit-btn">Submit Review</button>
                    </form>
                </div>
            </div>
        </section>

        <div class="ad-unit">
            <div class="container">
                <!-- Google AdSense In-Article Ad -->
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                     data-ad-slot="XXXXXXXXXX"
                     data-ad-format="fluid"
                     data-ad-layout="in-article"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
        </div>

        <section id="about" class="about-section">
            <div class="container">
                <h2>About Hyderabad Food Guide</h2>
                <div class="about-content">
                    <p>Hyderabad Food Guide is a passion project dedicated to exploring and documenting the rich culinary heritage of Hyderabad. From the iconic Hyderabadi Biryani to the hidden street food gems, we cover it all.</p>
                    <p>Our team of local food enthusiasts visits each establishment personally to bring you authentic reviews and recommendations.</p>
                </div>
            </div>
        </section>

        <section id="newsletter" class="newsletter-section">
            <div class="container">
                <h2>Subscribe to Our Food Newsletter</h2>
                <form id="newsletterForm">
                    <input type="email" placeholder="Your email address" required>
                    <button type="submit">Subscribe</button>
                </form>
                <p>Get weekly updates on new restaurant openings, food festivals, and exclusive discounts!</p>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-col">
                    <h3>Hyderabad Food Guide</h3>
                    <p>Your ultimate guide to Hyderabad's culinary landscape.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-facebook"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="footer-col">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#restaurants">Restaurants</a></li>
                        <li><a href="#street-food">Street Food</a></li>
                        <li><a href="#biryani-trail">Biryani Trail</a></li>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Popular Areas</h3>
                    <ul>
                        <li><a href="#">Banjara Hills</a></li>
                        <li><a href="#">Jubilee Hills</a></li>
                        <li><a href="#">Secunderabad</a></li>
                        <li><a href="#">Old City</a></li>
                        <li><a href="#">HITEC City</a></li>
                        <li><a href="#">Gachibowli</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Contact Us</h3>
                    <p>Email: contact@hyderabadfoodguide.com</p>
                    <p>Phone: +91 9876543210</p>
                    <p>Address: Food Street, Hyderabad, TS 500001</p>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; <span id="currentYear"></span> Hyderabad Food Guide. All rights reserved.</p>
                <ul>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms of Service</a></li>
                    <li><a href="#">Sitemap</a></li>
                </ul>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Mobile Menu Toggle
            const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
            const mainNav = document.querySelector('.main-nav');
            
            mobileMenuBtn.addEventListener('click', function() {
                this.classList.toggle('active');
                mainNav.classList.toggle('active');
            });
            
            // Close mobile menu when clicking on a link
            const navLinks = document.querySelectorAll('.main-nav ul li a');
            navLinks.forEach(link => {
                link.addEventListener('click', function() {
                    mobileMenuBtn.classList.remove('active');
                    mainNav.classList.remove('active');
                });
            });
            
            // Restaurant Data
            const restaurants = [
                {
                    id: 1,
                    name: "Paradise Biryani",
                    location: "Secunderabad",
                    description: "The most famous biryani in Hyderabad, known for its unique flavor and aroma.",
                    image: "https://source.unsplash.com/random/600x400/?biryani",
                    category: "biryani",
                    rating: 4.8,
                    price: "₹400-₹600",
                    tag: "Legendary"
                },
                {
                    id: 2,
                    name: "Bawarchi",
                    location: "RTC Cross Roads",
                    description: "Authentic Hyderabadi biryani with generous portions and rich flavors.",
                    image: "https://source.unsplash.com/random/600x400/?hyderabadi-biryani",
                    category: "biryani",
                    rating: 4.6,
                    price: "₹300-₹500",
                    tag: "Must Try"
                },
                {
                    id: 3,
                    name: "Ohri's Jiva Imperia",
                    location: "Jubilee Hills",
                    description: "Fine dining experience with a mix of Indian and international cuisines.",
                    image: "https://source.unsplash.com/random/600x400/?fine-dining",
                    category: "fine-dining",
                    rating: 4.5,
                    price: "₹1500-₹3000",
                    tag: "Luxury"
                },
                {
                    id: 4,
                    name: "Chutneys",
                    location: "Banjara Hills",
                    description: "Famous for its South Indian breakfast and meals in a contemporary setting.",
                    image: "https://source.unsplash.com/random/600x400/?dosa",
                    category: "vegetarian",
                    rating: 4.3,
                    price: "₹200-₹400",
                    tag: "Vegetarian"
                },
                {
                    id: 5,
                    name: "Cafe Bahar",
                    location: "Basheerbagh",
                    description: "Known for its delicious biryani and kebabs at reasonable prices.",
                    image: "https://source.unsplash.com/random/600x400/?kebab",
                    category: "biryani",
                    rating: 4.4,
                    price: "₹350-₹550",
                    tag: "Popular"
                },
                {
                    id: 6,
                    name: "Taj Mahal Tea House",
                    location: "Abids",
                    description: "Iconic Irani cafe known for its chai, Osmania biscuits and bun maska.",
                    image: "https://source.unsplash.com/random/600x400/?tea",
                    category: "cafe",
                    rating: 4.2,
                    price: "₹50-₹200",
                    tag: "Heritage"
                },
                {
                    id: 7,
                    name: "Minerva Coffee Shop",
                    location: "S.D. Road",
                    description: "Classic South Indian vegetarian restaurant with excellent filter coffee.",
                    image: "https://source.unsplash.com/random/600x400/?coffee",
                    category: "vegetarian",
                    rating: 4.1,
                    price: "₹100-₹300",
                    tag: "Breakfast"
                },
                {
                    id: 8,
                    name: "Fusion 9",
                    location: "Gachibowli",
                    description: "Multi-cuisine restaurant with a great ambience and innovative dishes.",
                    image: "https://source.unsplash.com/random/600x400/?fusion-food",
                    category: "fine-dining",
                    rating: 4.3,
                    price: "₹800-₹2000",
                    tag: "Modern"
                }
            ];
            
            // Featured Restaurants (top 4 by rating)
            const featuredRestaurants = [...restaurants]
                .sort((a, b) => b.rating - a.rating)
                .slice(0, 4);
            
            // Street Food Data
            const streetFoods = [
                {
                    id: 1,
                    name: "Irani Chai & Osmania Biscuit",
                    location: "Nampally",
                    description: "The perfect combination of sweet tea and buttery biscuits.",
                    icon: "☕"
                },
                {
                    id: 2,
                    name: "Haleem",
                    location: "Old City",
                    description: "Special Ramadan delicacy made with wheat, meat and spices.",
                    icon: "🍲"
                },
                {
                    id: 3,
                    name: "Double Ka Meetha",
                    location: "Charminar",
                    description: "Bread pudding dessert that's a Hyderabadi specialty.",
                    icon: "🍮"
                },
                {
                    id: 4,
                    name: "Mirchi Bajji",
                    location: "Koti",
                    description: "Deep fried chili fritters served with tangy chutneys.",
                    icon: "🌶️"
                },
                {
                    id: 5,
                    name: "Kebabs",
                    location: "Barkas",
                    description: "Juicy grilled meat skewers with Middle Eastern influences.",
                    icon: "🍢"
                },
                {
                    id: 6,
                    name: "Paya Soup",
                    location: "Tolichowki",
                    description: "Rich trotter soup eaten with naan or rumali roti.",
                    icon: "🥣"
                }
            ];
            
            // Biryani Guide Data
            const biryaniGuide = [
                {
                    id: 1,
                    name: "Hyderabadi Dum Biryani",
                    description: "The crown jewel of Hyderabadi cuisine, cooked with basmati rice, meat and a blend of spices in the dum style.",
                    type: "Mutton",
                    spiceLevel: "Medium-Hot",
                    price: "₹400-₹600"
                },
                {
                    id: 2,
                    name: "Kachi Dumm Biryani",
                    description: "Made with marinated raw meat layered with rice and cooked on low flame, resulting in incredibly tender meat.",
                    type: "Chicken/Mutton",
                    spiceLevel: "Medium",
                    price: "₹350-₹550"
                },
                {
                    id: 3,
                    name: "Prawn Biryani",
                    description: "Coastal influence on the classic with fresh prawns as the star ingredient.",
                    type: "Seafood",
                    spiceLevel: "Mild-Medium",
                    price: "₹450-₹650"
                },
                {
                    id: 4,
                    name: "Vegetable Biryani",
                    description: "Aromatic vegetarian version with mixed vegetables, sometimes with paneer or soya chunks.",
                    type: "Vegetarian",
                    spiceLevel: "Mild",
                    price: "₹250-₹400"
                }
            ];
            
            // Testimonials Data
            const testimonials = [
                {
                    id: 1,
                    name: "Rahul Sharma",
                    avatar: "https://randomuser.me/api/portraits/men/32.jpg",
                    rating: 5,
                    text: "The biryani at Paradise lives up to its reputation! The flavors are incredible and the meat is so tender.",
                    restaurant: "Paradise Biryani"
                },
                {
                    id: 2,
                    name: "Priya Patel",
                    avatar: "https://randomuser.me/api/portraits/women/44.jpg",
                    rating: 4,
                    text: "Chutneys has the best South Indian breakfast in town. Their pesarattu is to die for!",
                    restaurant: "Chutneys"
                },
                {
                    id: 3,
                    name: "Arjun Reddy",
                    avatar: "https://randomuser.me/api/portraits/men/67.jpg",
                    rating: 5,
                    text: "Bawarchi's biryani is my absolute favorite. The perfect balance of spices and the meat just falls off the bone.",
                    restaurant: "Bawarchi"
                },
                {
                    id: 4,
                    name: "Neha Gupta",
                    avatar: "https://randomuser.me/api/portraits/women/28.jpg",
                    rating: 4,
                    text: "Ohri's Jiva Imperia offers a fantastic fine dining experience. The ambience and food are both top-notch.",
                    restaurant: "Ohri's Jiva Imperia"
                },
                {
                    id: 5,
                    name: "Vikram Singh",
                    avatar: "https://randomuser.me/api/portraits/men/75.jpg",
                    rating: 5,
                    text: "The haleem during Ramadan in the Old City is something every food lover must experience at least once.",
                    restaurant: "Old City Haleem"
                }
            ];
            
            // Render Featured Restaurants
            const featuredContainer = document.getElementById('featuredRestaurants');
            
            featuredRestaurants.forEach(restaurant => {
                const stars = '★'.repeat(Math.round(restaurant.rating)) + '☆'.repeat(5 - Math.round(restaurant.rating));
                
                featuredContainer.innerHTML += `
                    <div class="featured-card">
                        <div class="featured-img">
                            <img src="${restaurant.image}" alt="${restaurant.name}">
                        </div>
                        <div class="featured-content">
                            <h3>${restaurant.name}</h3>
                            <p>${restaurant.description}</p>
                            <div class="featured-rating">
                                <span class="stars">${stars}</span>
                                <span>${restaurant.rating}/5</span>
                            </div>
                            <div class="featured-meta">
                                <span>${restaurant.location}</span>
                                <span>${restaurant.price}</span>
                            </div>
                        </div>
                    </div>
                `;
            });
            
            // Render All Restaurants
            const restaurantsGrid = document.getElementById('restaurantsGrid');
            
            function renderRestaurants(filter = 'all') {
                restaurantsGrid.innerHTML = '';
                
                const filtered = filter === 'all' 
                    ? restaurants 
                    : restaurants.filter(r => r.category === filter);
                
                filtered.forEach(restaurant => {
                    const stars = '★'.repeat(Math.round(restaurant.rating)) + '☆'.repeat(5 - Math.round(restaurant.rating));
                    
                    restaurantsGrid.innerHTML += `
                        <div class="restaurant-card" data-category="${restaurant.category}">
                            <div class="restaurant-img">
                                <img src="${restaurant.image}" alt="${restaurant.name}">
                                <span class="restaurant-tag">${restaurant.tag}</span>
                            </div>
                            <div class="restaurant-content">
                                <h3>${restaurant.name}</h3>
                                <div class="restaurant-location">
                                    <i class="fas fa-map-marker-alt"></i>
                                    <span>${restaurant.location}</span>
                                </div>
                                <p class="restaurant-desc">${restaurant.description}</p>
                                <div class="restaurant-footer">
                                    <div class="restaurant-rating">
                                        <span class="stars">${stars}</span>
                                        <span>${restaurant.rating}</span>
                                    </div>
                                    <div class="restaurant-price">${restaurant.price}</div>
                                </div>
                            </div>
                        </div>
                    `;
                });
            }
            
            renderRestaurants();
            
            // Filter Restaurants
            const filterBtns = document.querySelectorAll('.filter-btn');
            
            filterBtns.forEach(btn => {
                btn.addEventListener('click', function() {
                    filterBtns.forEach(b => b.classList.remove('active'));
                    this.classList.add('active');
                    
                    const filter = this.getAttribute('data-filter');
                    renderRestaurants(filter);
                });
            });
            
            // Render Street Food
            const streetFoodList = document.getElementById('streetFoodList');
            
            streetFoods.forEach(food => {
                streetFoodList.innerHTML += `
                    <div class="street-food-item">
                        <div class="street-food-icon">${food.icon}</div>
                        <div class="street-food-content">
                            <h4>${food.name}</h4>
                            <p>${food.location} • ${food.description}</p>
                        </div>
                    </div>
                `;
            });
            
            // Render Biryani Guide
            const biryaniGuideContainer = document.getElementById('biryaniGuide');
            
            biryaniGuide.forEach(item => {
                biryaniGuideContainer.innerHTML += `
                    <div class="biryani-card">
                        <h3>${item.name}</h3>
                        <p>${item.description}</p>
                        <div class="biryani-specs">
                            <div class="biryani-spec">
                                <i class="fas fa-utensils"></i>
                                <span>${item.type}</span>
                            </div>
                            <div class="biryani-spec">
                                <i class="fas fa-pepper-hot"></i>
                                <span>${item.spiceLevel}</span>
                            </div>
                        </div>
                        <div class="biryani-price">${item.price}</div>
                    </div>
                `;
            });
            
            // Render Testimonials
            const testimonialsSlider = document.getElementById('testimonialsSlider');
            
            testimonials.forEach(testimonial => {
                const stars = '★'.repeat(testimonial.rating) + '☆'.repeat(5 - testimonial.rating);
                
                testimonialsSlider.innerHTML += `
                    <div class="testimonial-card">
                        <div class="testimonial-header">
                            <div class="testimonial-avatar">
                                <img src="${testimonial.avatar}" alt="${testimonial.name}">
                            </div>
                            <div class="testimonial-user">
                                <h4>${testimonial.name}</h4>
                                <div class="testimonial-rating">${stars}</div>
                            </div>
                        </div>
                        <p class="testimonial-text">"${testimonial.text}"</p>
                        <p class="testimonial-restaurant">Visited <a href="#">${testimonial.restaurant}</a></p>
                    </div>
                `;
            });
            
            // Populate Restaurant Select in Testimonial Form
            const restaurantSelect = document.getElementById('restaurantVisited');
            
            restaurants.forEach(restaurant => {
                restaurantSelect.innerHTML += `
                    <option value="${restaurant.id}">${restaurant.name}</option>
                `;
            });
            
            // Star Rating in Testimonial Form
            const stars = document.querySelectorAll('.star-rating .star');
            const ratingInput = document.getElementById('userRating');
            
            stars.forEach(star => {
                star.addEventListener('click', function() {
                    const value = parseInt(this.getAttribute('data-value'));
                    ratingInput.value = value;
                    
                    stars.forEach(s => {
                        s.classList.remove('active');
                        if (parseInt(s.getAttribute('data-value')) <= value) {
                            s.classList.add('active');
                        }
                    });
                });
            });
            
            // Testimonial Form Submission
            const testimonialForm = document.getElementById('testimonialForm');
            
            testimonialForm.addEventListener('submit', function(e) {
                e.preventDefault();
                
                const name = document.getElementById('userName').value;
                const email = document.getElementById('userEmail').value;
                const text = document.getElementById('userTestimonial').value;
                const restaurantId = document.getElementById('restaurantVisited').value;
                const rating = document.getElementById('userRating').value;
                
                if (!name || !text || rating === '0') {
                    alert('Please fill all required fields and provide a rating');
                    return;
                }
                
                const restaurant = restaurants.find(r => r.id === parseInt(restaurantId)) || { name: 'Various locations' };
                
                // Create new testimonial
                const newTestimonial = {
                    id: testimonials.length + 1,
                    name: name,
                    avatar: `https://ui-avatars.com/api/?name=${encodeURIComponent(name)}&background=random`,
                    rating: parseInt(rating),
                    text: text,
                    restaurant: restaurant.name
                };
                
                // Add to testimonials array
                testimonials.push(newTestimonial);
                
                // Add to slider
                const stars = '★'.repeat(newTestimonial.rating) + '☆'.repeat(5 - newTestimonial.rating);
                
                testimonialsSlider.innerHTML += `
                    <div class="testimonial-card">
                        <div class="testimonial-header">
                            <div class="testimonial-avatar">
                                <img src="${newTestimonial.avatar}" alt="${newTestimonial.name}">
                            </div>
                            <div class="testimonial-user">
                                <h4>${newTestimonial.name}</h4>
                                <div class="testimonial-rating">${stars}</div>
                            </div>
                        </div>
                        <p class="testimonial-text">"${newTestimonial.text}"</p>
                        <p class="testimonial-restaurant">Visited <a href="#">${newTestimonial.restaurant}</a></p>
                    </div>
                `;
                
                // Reset form
                testimonialForm.reset();
                stars.forEach(s => s.classList.remove('active'));
                ratingInput.value = '0';
                
                // Scroll to new testimonial
                testimonialsSlider.scrollTo({
                    left: testimonialsSlider.scrollWidth,
                    behavior: 'smooth'
                });
                
                // Show success message
                alert('Thank you for your testimonial!');
            });
            
            // Newsletter Form Submission
            const newsletterForm = document.getElementById('newsletterForm');
            
            newsletterForm.addEventListener('submit', function(e) {
                e.preventDefault();
                const email = this.querySelector('input').value;
                
                // In a real app, you would send this to your server
                console.log('New newsletter subscription:', email);
                
                // Show success message
                alert('Thank you for subscribing to our newsletter!');
                this.reset();
            });
            
            // Smooth scrolling for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    const targetId = this.getAttribute('href');
                    if (targetId === '#') return;
                    
                    const targetElement = document.querySelector(targetId);
                    if (targetElement) {
                        const headerHeight = document.querySelector('.header').offsetHeight;
                        const targetPosition = targetElement.offsetTop - headerHeight;
                        
                        window.scrollTo({
                            top: targetPosition,
                            behavior: 'smooth'
                        });
                    }
                });
            });
            
            // Set current year in footer
            document.getElementById('currentYear').textContent = new Date().getFullYear();
        });
    </script>
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <!-- Schema.org markup for Google -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "WebSite",
      "name": "Hyderabad Food Guide",
      "url": "https://example.com",
      "potentialAction": {
        "@type": "SearchAction",
        "target": "https://example.com/search?q={search_term_string}",
        "query-input": "required name=search_term_string"
      }
    }
    </script>
</body>
</html>
