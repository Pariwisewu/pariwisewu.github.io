<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PARIWISEWU</title>
    <style>
        .video-container {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            margin-top: 20px;
        }
        iframe {
            width: 480px;
            height: 270px;
            max-width: 100%;
        }
        .hero {
            position: relative;
            width: 100%;
            height: 100vh;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            /* text-align: center; */
        }
        .carousel {
            position: absolute;
            width: 100%;
            height: 100%;
            z-index: -1;
        }
        .carousel img {
            position: absolute;
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0;
            transition: opacity 1s ease-in-out;
        }
        .carousel img.active {
            opacity: 1;
        }
        .hero-content {
            position: relative;
            z-index: 1;
            background: rgba(0, 0, 0, 0.5);
            padding: 20px;
            border-radius: 10px;
        }
        .cta-button {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 20px;
            background: #ff9800;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }

        /* Variabel warna */
        :root {
            --pringsewu-green: #0D6832;
            --pringsewu-gold: #D4AF37;
            --dark-green: #084d25;
            --light-green: #1e8d4b;
            --light-gold: #e9cb69;
            --white: #ffffff;
            --black: #333333;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f5f5f5;
            color: var(--black);
        }

        header {
            background-color: var(--pringsewu-green);
            padding: 20px 0;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            position: relative;
            z-index: 100;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo h1 {
            color: var(--white);
            font-size: 1.8rem;
            margin-left: 15px;
        }

        .logo span {
            color: var(--pringsewu-gold);
        }

        .logo-img {
            width: 50px;
            height: 50px;
            background-color: var(--pringsewu-gold);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            color: var(--pringsewu-green);
            font-size: 20px;
        }

        nav {
            position: relative;
        }

        .nav-toggle {
            display: none;
            color: var(--white);
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
        }

        .main-menu {
            display: flex;
            list-style: none;
        }

        .main-menu > li {
            position: relative;
            margin-left: 20px;
        }

        .main-menu > li > a {
            color: var(--white);
            text-decoration: none;
            padding: 10px 15px;
            display: block;
            font-weight: 500;
            transition: all 0.3s ease;
            border-radius: 5px;
        }

        .main-menu > li > a:hover {
            background-color: var(--dark-green);
            color: var(--pringsewu-gold);
        }

        .sub-menu {
            position: absolute;
            top: 100%;
            left: 0;
            background-color: var(--white);
            border-radius: 5px;
            min-width: 200px;
            padding: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            display: none;
            transition: all 0.3s ease;
            z-index: 999;
        }

        .sub-menu li {
            list-style: none;
        }

        .sub-menu li a {
            color: var(--black);
            text-decoration: none;
            padding: 8px 10px;
            display: block;
            border-radius: 3px;
            transition: all 0.3s ease;
        }

        .sub-menu li a:hover {
            background-color: var(--light-green);
            color: var(--white);
        }

        .main-menu > li:hover .sub-menu {
            display: block;
            animation: fadeIn 0.3s ease forwards;
        }

        /* Hero Section */
        /* .hero {
            height: 70vh;
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/api/placeholder/1200/800') center/cover no-repeat;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--white);
        } */

        .hero-content {
            max-width: 800px;
            padding: 20px;
        }

        .hero h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
        }

        .cta-button {
            display: inline-block;
            background-color: var(--pringsewu-gold);
            color: var(--dark-green);
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            border: 2px solid var(--pringsewu-gold);
        }

        .cta-button:hover {
            background-color: transparent;
            color: var(--pringsewu-gold);
        }

        /* Highlight Section */
        .highlight-section, .concept-section, .package-section {
            padding: 60px 0;
            background-color: var(--white);
        }

        .highlight-section:nth-child(even), .concept-section:nth-child(even) {
            background-color: #f5f5f5;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: var(--pringsewu-green);
            position: relative;
        }

        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 3px;
            background-color: var(--pringsewu-gold);
            margin: 15px auto;
        }

        .card-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 25px;
        }

        .card {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-10px);
        }

        .card-img {
            height: 200px;
            background: url('/api/placeholder/400/300') center/cover no-repeat;
        }

        .card-content {
            padding: 20px;
        }

        .card h3 {
            color: var(--pringsewu-green);
            margin-bottom: 10px;
        }

        .card p {
            color: var(--black);
            margin-bottom: 15px;
            font-size: 0.9rem;
            line-height: 1.4;
        }

        .card-link {
            display: inline-block;
            color: var(--pringsewu-gold);
            font-weight: 500;
            text-decoration: none;
        }

        .card-link:hover {
            text-decoration: underline;
        }

        /* Konsep 5A */
        .concept-box {
            padding: 30px;
            background-color: var(--white);
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            margin-bottom: 30px;
        }

        .concept-intro {
            text-align: center;
            margin-bottom: 40px;
        }

        .concept-intro p {
            font-size: 1.1rem;
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.6;
        }

        .concept-items {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .concept-item {
            padding: 20px;
            border-radius: 10px;
            background-color: rgba(13, 104, 50, 0.05);
            text-align: center;
            transition: all 0.3s ease;
        }

        .concept-item:hover {
            background-color: rgba(212, 175, 55, 0.1);
            transform: translateY(-5px);
        }

        .concept-item h3 {
            color: var(--pringsewu-green);
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .concept-item p {
            font-size: 0.9rem;
            line-height: 1.5;
        }

        .concept-icon {
            font-size: 2rem;
            color: var(--pringsewu-gold);
            margin-bottom: 15px;
        }

        /* Package Details */
        .package-detail {
            display: none;
            padding: 20px;
            background-color: var(--white);
            border-radius: 10px;
            margin-top: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .package-detail.active {
            display: block;
            animation: fadeIn 0.5s ease forwards;
        }

        .package-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 1px solid rgba(0, 0, 0, 0.1);
        }

        .package-price {
            background-color: var(--pringsewu-gold);
            color: var(--white);
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: bold;
        }

        .package-info {
            margin-bottom: 20px;
        }

        .package-info-item {
            margin-bottom: 10px;
            display: flex;
            align-items: flex-start;
        }

        .package-info-item strong {
            min-width: 100px;
            display: inline-block;
        }

        .package-destinations {
            list-style: none;
            margin-bottom: 20px;
        }

        .package-destinations li {
            padding: 5px 0;
            position: relative;
            padding-left: 20px;
        }

        .package-destinations li:before {
            content: '•';
            color: var(--pringsewu-gold);
            position: absolute;
            left: 0;
            font-size: 1.2rem;
        }

        .rundown-title {
            font-weight: bold;
            margin: 15px 0 10px;
            color: var(--pringsewu-green);
        }

        .rundown-list {
            list-style: none;
            margin-bottom: 20px;
        }

        .rundown-list li {
            padding: 5px 0;
            position: relative;
            padding-left: 80px;
        }

        .rundown-list li:before {
            content: attr(data-time);
            position: absolute;
            left: 0;
            font-weight: bold;
        }

        .package-facilities {
            list-style: none;
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 20px;
        }

        .package-facilities li {
            background-color: rgba(13, 104, 50, 0.1);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
        }

        .close-package {
            background-color: var(--pringsewu-green);
            color: var(--white);
            border: none;
            padding: 8px 20px;
            border-radius: 5px;
            margin-top: 20px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .close-package:hover {
            background-color: var(--dark-green);
        }

        /* Footer */
        footer {
            background-color: var(--pringsewu-green);
            color: var(--white);
            padding: 40px 0 20px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
        }

        .footer-column h3 {
            color: var(--pringsewu-gold);
            margin-bottom: 20px;
            position: relative;
        }

        .footer-column h3:after {
            content: '';
            display: block;
            width: 40px;
            height: 2px;
            background-color: var(--pringsewu-gold);
            margin-top: 10px;
        }

        .footer-column ul {
            list-style: none;
        }

        .footer-column ul li {
            margin-bottom: 10px;
        }

        .footer-column ul li a {
            color: var(--white);
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .footer-column ul li a:hover {
            color: var(--pringsewu-gold);
            padding-left: 5px;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 35px;
            height: 35px;
            background-color: var(--light-green);
            color: var(--white);
            border-radius: 50%;
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            background-color: var(--pringsewu-gold);
            color: var(--pringsewu-green);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            margin-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.7);
        }

        /* Animasi */
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(10px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Media Queries for Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                align-items: flex-start;
            }

            .nav-toggle {
                display: block;
                position: absolute;
                top: 15px;
                right: 15px;
            }

            .main-menu {
                display: none;
                flex-direction: column;
                width: 100%;
                margin-top: 20px;
            }

            .main-menu.active {
                display: flex;
            }

            .main-menu > li {
                margin: 0;
                width: 100%;
            }

            .main-menu > li > a {
                padding: 12px 0;
            }

            .sub-menu {
                position: static;
                width: 100%;
                box-shadow: none;
                padding: 0 0 0 20px;
            }

            .hero {
                height: 60vh;
            }

            .hero h2 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .concept-items {
                grid-template-columns: 1fr;
            }

            .package-header {
                flex-direction: column;
                align-items: flex-start;
            }

            .package-price {
                margin-top: 10px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <img src="gambar/logo.png" alt="Logo Pariwisewu" class="logo-img">
                    <h1>Pariwi<span>Sewu</span></h1>
                </div>
                <button class="nav-toggle" onclick="toggleMenu()">☰</button>
                <nav>
                    <ul class="main-menu" id="mainMenu">
                        <li>
                            <a href="#">Wisata</a>
                            <ul class="sub-menu">
                                <li><a href="#" onclick="showPackage('alam')">Wisata Alam</a></li>
                                <li><a href="#" onclick="showPackage('religi')">Religi & Sejarah</a></li>
                                <li><a href="#" onclick="showPackage('kuliner')">Kuliner</a></li>
                                <li><a href="#" onclick="showPackage('edukasi')">Edukasi & Budaya</a></li>
                                <li><a href="#" onclick="showPackage('adventure')">Adventure</a></li>
                                <li><a href="#" onclick="showPackage('keluarga')">Keluarga</a></li>
                                <li><a href="#" onclick="showPackage('komplit')">Paket Komplit</a></li>
                            </ul>
                        </li>
                        <li><a href="https://www.canva.com/design/DAGhWGsmz54/ndH4PIUD9CmvonmHxqqKgA/view?utm_content=DAGhWGsmz54&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h4b937c3105" target="_blank">Denah Wisata Pringsewu</a></li>
                        <li><a href="https://www.instagram.com/pariwisewu" target="_blank">Informasi UMKM</a></li>
                        <li>
                            <a href="#">Kontak</a>
                            <ul class="sub-menu">
                                <li><a href="https://wa.me/6285658987525" target="_blank">Mifta</a></li>
                                <li><a href="https://wa.me/6285839227740" target="_blank">Aufar</a></li>
                            </ul>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <section class="hero">
        <div class="carousel">
            <img src="gambar/gambar1.jpg" class="active" alt="Pringsewu 1">
            <img src="gambar/gambar3.jpg" alt="Pringsewu 2">
            <img src="gambar/gambar4.jpg" alt="Pringsewu 3">
        </div>
        <div class="hero-content">
            <h2>Jelajahi Keindahan Pringsewu</h2>
            <p>Temukan destinasi wisata menarik, kuliner lezat, dan kebudayaan unik di kabupaten Pringsewu. Kami menyediakan berbagai paket wisata untuk pengalaman liburan terbaik Anda.</p>
            <a href="#packages" class="cta-button">Lihat Paket Wisata</a>
        </div>
    </section>
    <div class="video-container">
        <iframe src="https://www.youtube.com/embed/IohtewHolZc?si=rUtvOKgB4SExN3E3" frameborder="0" allowfullscreen></iframe>
        <iframe src="https://www.youtube.com/embed/Yh7WGkg2ZWU?si=p5tvvjdUZHq_-HGB" frameborder="0" allowfullscreen></iframe>
    </div>
    <section class="concept-section">
        <div class="container">
            <h2 class="section-title">Tentang Kami Pariwisewu</h2>
            <div class="concept-box">
                <div class="concept-intro">
                    <p>Pariwisewu adalah jasa tour leader kece di Pringsewu yang ngajak kamu eksplor wisata, kuliner, dan kerajinan lokal sambil dukung ekonomi daerah. Nggak cuma jalan-jalan, tapi juga seru-seruan sambil kenal lebih dekat sama budaya Pringsewu. Yuk, wisata asik sambil bantu UMKM bareng Pariwisewu! 🚀✨</p>
                </div>

                <div class="concept-items">
                    <div class="concept-item">
                        <div class="concept-icon">🏞️</div>
                        <h3>Atraksi</h3>
                        <p>PARIWISEWU mengajak wisatawan mengeksplor keindahan alam Pringsewu, seperti bukit, air terjun, dan sawah hijau, serta mengenalkan budaya lokal lewat seni, tradisi, dan sejarah daerah.</p>
                    </div>
                    
                    <div class="concept-item">
                        <div class="concept-icon">🏨</div>
                        <h3>Akomodasi</h3>
                        <p>PARIWISEWU membantu wisatawan menemukan tempat menginap yang nyaman, mulai dari homestay, villa, hingga hotel berbintang, sesuai dengan kebutuhan dan budget.</p>
                    </div>
                    
                    <div class="concept-item">
                        <div class="concept-icon">🚌</div>
                        <h3>Aksesibilitas</h3>
                        <p>Dengan rute perjalanan yang dirancang efisien, PARIWISEWU memastikan wisatawan mendapatkan transportasi yang nyaman, baik kendaraan pribadi, umum, maupun layanan antar-jemput.</p>
                    </div>
                    
                    <div class="concept-item">
                        <div class="concept-icon">🧗‍♂️</div>
                        <h3>Aktivitas</h3>
                        <p>PARIWISEWU menawarkan pengalaman seru seperti wisata petualangan, kuliner, belanja oleh-oleh khas, hingga workshop budaya dan kerajinan lokal.</p>
                    </div>
                    
                    <div class="concept-item">
                        <div class="concept-icon">🍽️</div>
                        <h3>Amenitas</h3>
                        <p>Wisatawan tidak perlu khawatir, karena PARIWISEWU merekomendasikan berbagai fasilitas pendukung seperti restoran khas, pusat oleh-oleh, layanan kesehatan, hingga informasi wisata yang lengkap.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="highlight-section" id="packages">
        <div class="container">
            <h2 class="section-title">Paket Wisata Pringsewu</h2>
            <div class="card-container">
                <div class="card" onclick="showPackage('alam')">
                    <div class="card-img" style="background-image: url(gambar/gambar5.jpg);"></div>
                    <div class="card-content">
                        <h3>Wisata Alam</h3>
                        <p>Nikmati keindahan alam Pringsewu dengan pemandangan yang menyegarkan mata dan udara yang sejuk.</p>
                        <a href="#" class="card-link">Lihat Detail →</a>
                    </div>
                </div>

                <div class="card" onclick="showPackage('religi')">
                    <div class="card-img" style="background-image: url(gambar/religi.jpg);"></div>
                    <div class="card-content">
                        <h3>Religi & Sejarah</h3>
                        <p>Jelajahi tempat-tempat bersejarah dan religi di Pringsewu yang kaya akan nilai budaya dan spiritual.</p>
                        <a href="#" class="card-link">Lihat Detail →</a>
                    </div>
                </div>

                <div class="card" onclick="showPackage('kuliner')">
                    <div class="card-img" style="background-image: url(gambar/kuliner.jpg);"></div>
                    <div class="card-content">
                        <h3>Kuliner Khas</h3>
                        <p>Cicipi berbagai kuliner khas Pringsewu yang akan memanjakan lidah Anda dengan cita rasa yang unik.</p>
                        <a href="#" class="card-link">Lihat Detail →</a>
                    </div>
                </div>

                <div class="card" onclick="showPackage('edukasi')">
                    <div class="card-img" style="background-image: url(gambar/pengrajin.jpg);"></div>
                    <div class="card-content">
                        <h3>Edukasi & Budaya</h3>
                        <p>Kunjungi tempat-tempat edukasi yang menarik dan menambah wawasan tentang budaya Pringsewu.</p>
                        <a href="#" class="card-link">Lihat Detail →</a>
                    </div>
                </div>
                
                <div class="card" onclick="showPackage('adventure')">
                    <div class="card-img" style="background-image: url(gambar/outboand.jpeg);"></div>
                    <div class="card-content">
                        <h3>Outbound & Adventure</h3>
                        <p>Tantang adrenalin Anda dengan berbagai petualangan seru di alam Pringsewu.</p>
                        <a href="#" class="card-link">Lihat Detail →</a>
                    </div>
                </div>
                
                <div class="card" onclick="showPackage('keluarga')">
                    <div class="card-img" style="background-image: url(gambar/keluarga.jpg);"></div>
                    <div class="card-content">
                        <h3>Wisata Keluarga</h3>
                        <p>Nikmati liburan bersama keluarga dengan mengunjungi tempat-tempat wisata ramah keluarga di Pringsewu.</p>
                        <a href="#" class="card-link">Lihat Detail →</a>
                    </div>
                </div>
                
                <div class="card" onclick="showPackage('komplit')">
                    <div class="card-img" style="background-image: url(gambar/komplit.jpeg);"></div>
                    <div class="card-content">
                        <h3>Paket Komplit</h3>
                        <p>Nikmati pengalaman lengkap berwisata di Pringsewu selama 3 hari 2 malam dengan mengunjungi berbagai destinasi menarik.</p>
                        <a href="#" class="card-link">Lihat Detail →</a>
                    </div>
                </div>
            </div>
            
            <!-- Package Details Sections -->
            <div id="packageDetails">
                <!-- Paket Wisata Alam -->
                <div id="alam" class="package-detail">
                    <div class="package-header">
                        <h3>Paket Wisata Alam Pringsewu 🌿</h3>
                        <div class="package-price">Rp250.000/orang</div>
                    </div>
                    
                    <div class="package-info">
                        <div class="package-info-item">
                            <strong>Durasi:</strong> <span>1 Hari</span>
                        </div>
                        <div class="package-info-item">
                            <strong>Minimal:</strong> <span>5 orang</span>
                        </div>
                    </div>
                    
                    <h4>Destinasi:</h4>
                    <ul class="package-destinations">
                        <li>Bukit Pangonan (spot foto, trekking ringan)</li>
                        <li>Talang Indah (wisata sejarah & alam)</li>
                        <li>Hutan Kota Pringsewu (rekreasi & edukasi lingkungan)</li>
                    </ul>
                    
                    <h4 class="rundown-title">Rundown:</h4>
                    <ul class="rundown-list">
                        <li data-time="08.00">Penjemputan peserta</li>
                        <li data-time="09.00">Explore Bukit Pangonan</li>
                        <li data-time="11.00">Kunjungan ke Talang Indah</li>
                        <li data-time="12.00">Makan siang</li>
                        <li data-time="13.00">Wisata Hutan Kota Pringsewu</li>
                        <li data-time="15.00">Kembali ke titik awal</li>
                    </ul>
                    
                    <h4>Fasilitas:</h4>
                    <ul class="package-facilities">
                        <li>Transportasi lokal</li>
                        <li>Tiket masuk semua destinasi</li>
                        <li>Makan siang</li>
                        <li>Guide wisata</li>
                        <li>Dokumentasi</li>
                    </ul>
                    
                    <button class="close-package" onclick="closePackage()">Tutup</button>
                </div>
                
                <!-- Paket Wisata Religi & Sejarah -->
                <div id="religi" class="package-detail">
                    <div class="package-header">
                        <h3>Paket Wisata Religi & Sejarah 🕌🏛️</h3>
                        <div class="package-price">Rp200.000/orang</div>
                    </div>
                    
                    <div class="package-info">
                        <div class="package-info-item">
                            <strong>Durasi:</strong> <span>1 Hari</span>
                        </div>
                        <div class="package-info-item">
                            <strong>Minimal:</strong> <span>5 orang</span>
                        </div>
                    </div>
                    
                    <h4>Destinasi:</h4>
                    <ul class="package-destinations">
                        <li>Masjid Al-Muqorrobin (sejarah Islam di Pringsewu)</li>
                        <li>Vihara Vajra Bumi Kertayuga (wisata religi & arsitektur)</li>
                        <li>Tugu Gajah (ikon sejarah Pringsewu)</li>
                    </ul>
                    
                    <h4 class="rundown-title">Rundown:</h4>
                    <ul class="rundown-list">
                        <li data-time="08.00">Penjemputan peserta</li>
                        <li data-time="09.00">Kunjungan ke Masjid Al-Muqorrobin</li>
                        <li data-time="10.00">Explore Vihara Vajra Bumi Kertayuga</li>
                        <li data-time="11.30">Makan siang</li>
                        <li data-time="13.00">Kunjungan ke Tugu Gajah</li>
                        <li data-time="14.30">Kembali ke titik awal</li>
                    </ul>
                    
                    <h4>Fasilitas:</h4>
                    <ul class="package-facilities">
                        <li>Transportasi lokal</li>
                        <li>Tiket masuk semua destinasi</li>
                        <li>Makan siang</li>
                        <li>Guide wisata</li>
                        <li>Air mineral</li>
                    </ul>
                    
                    <button class="close-package" onclick="closePackage()">Tutup</button>
                </div>
                
                <!-- Paket Wisata Kuliner -->
                <div id="kuliner" class="package-detail">
                    <div class="package-header">
                        <h3>Paket Wisata Kuliner Pringsewu 🍽️</h3>
                        <div class="package-price">Rp275.000/orang</div>
                    </div>
                    
                    <div class="package-info">
                        <div class="package-info-item">
                            <strong>Durasi:</strong> <span>1 Hari</span>
                        </div>
                        <div class="package-info-item">
                            <strong>Minimal:</strong> <span>4 orang</span>
                        </div>
                    </div>
                    
                    <h4>Destinasi:</h4>
                    <ul class="package-destinations">
                        <li>Pasar Tradisional Pringsewu (belanja bahan masakan lokal)</li>
                        <li>Rumah Makan Ayam Panggang Bu Siti</li>
                        <li>Warung Seblak Jeletot Bang Ncep</li>
                        <li>Pusat Oleh-oleh Khas Pringsewu</li>
                    </ul>
                    
                    <h4 class="rundown-title">Rundown:</h4>
                    <ul class="rundown-list">
                        <li data-time="08.00">Penjemputan peserta</li>
                        <li data-time="08.30">Explore Pasar Tradisional Pringsewu</li>
                        <li data-time="10.30">Makan di Rumah Makan Ayam Panggang Bu Siti</li>
                        <li data-time="12.30">Mencicipi Seblak Jeletot Bang Ncep</li>
                        <li data-time="14.00">Belanja di Pusat Oleh-oleh Khas Pringsewu</li>
                        <li data-time="15.30">Kembali ke titik awal</li>
                    </ul>
                    
                    <h4>Fasilitas:</h4>
                    <ul class="package-facilities">
                        <li>Transportasi lokal</li>
                        <li>Makan di 2 tempat kuliner</li>
                        <li>Guide wisata</li>
                        <li>Voucher belanja oleh-oleh</li>
                        <li>Air mineral</li>
                    </ul>
                    
                    <button class="close-package" onclick="closePackage()">Tutup</button>
                </div>
                
                <!-- Paket Wisata Edukasi & Budaya -->
                <div id="edukasi" class="package-detail">
                    <div class="package-header">
                        <h3>Paket Wisata Edukasi & Budaya 📚🎭</h3>
                        <div class="package-price">Rp230.000/orang</div>
                    </div>
                    
                    <div class="package-info">
                        <div class="package-info-item">
                            <strong>Durasi:</strong> <span>1 Hari</span>
                        </div>
                        <div class="package-info-item">
                            <strong>Minimal:</strong> <span>6 orang</span>
                        </div>
                    </div>
                    
                    <h4>Destinasi:</h4>
                    <ul class="package-destinations">
                        <li>Perpustakaan Daerah Pringsewu</li>
                        <li>Kampung Batik Pringsewu (workshop membatik)</li>
                        <li>Sanggar Seni Tradisional (pertunjukan tari)</li>
                        <li>Pusat Kerajinan Tangan</li>
                    </ul>
                    
                    <h4 class="rundown-title">Rundown:</h4>
                    <ul class="rundown-list">
                        <li data-time="08.00">Penjemputan peserta</li>
                        <li data-time="08.30">Kunjungan ke Perpustakaan Daerah</li>
                        <li data-time="10.00">Workshop membatik di Kampung Batik</li>
                        <li data-time="12.00">Makan siang</li>
                        <li data-time="13.00">Pertunjukan tari di Sanggar Seni</li>
                        <li data-time="14.30">Belanja di Pusat Kerajinan Tangan</li>
                        <li data-time="16.00">Kembali ke titik awal</li>
                    </ul>
                    
                    <h4>Fasilitas:</h4>
                    <ul class="package-facilities">
                        <li>Transportasi lokal</li>
                        <li>Tiket masuk semua destinasi</li>
                        <li>Makan siang</li>
                        <li>Workshop membatik</li>
                        <li>Pertunjukan seni</li>
                        <li>Guide wisata</li>
                    </ul>
                    
                    <button class="close-package" onclick="closePackage()">Tutup</button>
                </div>
                
                <!-- Paket Outbound & Adventure -->
                <div id="adventure" class="package-detail">
                    <div class="package-header">
                        <h3>Paket Outbound & Adventure 🧗‍♂️🚵‍♀️</h3>
                        <div class="package-price">Rp300.000/orang</div>
                    </div>
                    
                    <div class="package-info">
                        <div class="package-info-item">
                            <strong>Durasi:</strong> <span>1 Hari</span>
                        </div>
                        <div class="package-info-item">
                            <strong>Minimal:</strong> <span>8 orang</span>
                        </div>
                    </div>
                    
                    <h4>Destinasi:</h4>
                    <ul class="package-destinations">
                        <li>Area Outbound Sungai Way Sekampung</li>
                        <li>Trekking Bukit Pangonan</li>
                        <li>Camping Area Hutan Pinus</li>
                    </ul>
                    
                    <h4 class="rundown-title">Rundown:</h4>
                    <ul class="rundown-list">
                        <li data-time="07.00">Penjemputan peserta</li>
                        <li data-time="08.00">Team building & outbound di Sungai Way Sekampung</li>
                        <li data-time="11.00">Makan siang</li>
                        <li data-time="12.00">Trekking Bukit Pangonan</li>
                        <li data-time="14.00">BBQ di Camping Area Hutan Pinus</li>
                        <li data-time="16.00">Kembali ke titik awal</li>
                    </ul>
                    
                    <h4>Fasilitas:</h4>
                    <ul class="package-facilities">
                        <li>Transportasi lokal</li>
                        <li>Peralatan outbound</li>
                        <li>Makan siang & BBQ</li>
                        <li>Guide profesional</li>
                        <li>P3K</li>
                        <li>Asuransi</li>
                        <li>Dokumentasi</li>
                    </ul>
                    
                    <button class="close-package" onclick="closePackage()">Tutup</button>
                </div>
                
                <!-- Paket Wisata Keluarga -->
                <div id="keluarga" class="package-detail">
                    <div class="package-header">
                        <h3>Paket Wisata Keluarga 👨‍👩‍👧‍👦</h3>
                        <div class="package-price">Rp260.000/orang</div>
                    </div>
                    
                    <div class="package-info">
                        <div class="package-info-item">
                            <strong>Durasi:</strong> <span>1 Hari</span>
                        </div>
                        <div class="package-info-item">
                            <strong>Minimal:</strong> <span>4 orang</span>
                        </div>
                    </div>
                    
                    <h4>Destinasi:</h4>
                    <ul class="package-destinations">
                        <li>Taman Wisata Keluarga</li>
                        <li>Kolam Renang Permata</li>
                        <li>Pusat Kuliner Keluarga</li>
                        <li>Pusat Oleh-oleh Khas Pringsewu</li>
                    </ul>
                    
                    <h4 class="rundown-title">Rundown:</h4>
                    <ul class="rundown-list">
                        <li data-time="08.00">Penjemputan peserta</li>
                        <li data-time="09.00">Bermain di Taman Wisata Keluarga</li>
                        <li data-time="11.30">Berenang di Kolam Renang Permata</li>
                        <li data-time="13.00">Makan siang di Pusat Kuliner Keluarga</li>
                        <li data-time="14.30">Belanja di Pusat Oleh-oleh</li>
                        <li data-time="16.00">Kembali ke titik awal</li>
                    </ul>
                    
                    <h4>Fasilitas:</h4>
                    <ul class="package-facilities">
                        <li>Transportasi lokal</li>
                        <li>Tiket masuk semua destinasi</li>
                        <li>Makan siang</li>
                        <li>Guide wisata</li>
                        <li>Dokumentasi</li>
                        <li>Air mineral</li>
                    </ul>
                    
                    <button class="close-package" onclick="closePackage()">Tutup</button>
                </div>
                
                <!-- Paket Komplit -->
                <div id="komplit" class="package-detail">
                    <div class="package-header">
                        <h3>Paket Wisata Komplit Pringsewu 🌟</h3>
                        <div class="package-price">Rp750.000/orang</div>
                    </div>
                    
                    <div class="package-info">
                        <div class="package-info-item">
                            <strong>Durasi:</strong> <span>3 Hari 2 Malam</span>
                        </div>
                        <div class="package-info-item">
                            <strong>Minimal:</strong> <span>10 orang</span>
                        </div>
                    </div>
                    
                    <h4>Destinasi:</h4>
                    <ul class="package-destinations">
                        <li>Semua destinasi unggulan di Pringsewu</li>
                        <li>Wisata alam (Bukit Pangonan, Talang Indah)</li>
                        <li>Wisata budaya & edukasi (Kampung Batik, Sanggar Seni)</li>
                        <li>Wisata kuliner khas Pringsewu</li>
                        <li>Outbound & adventure</li>
                    </ul>
                    
                    <h4 class="rundown-title">Rundown:</h4>
                    <p>Agenda 3 hari penuh dengan pengalaman wisata terbaik di Pringsewu. Jadwal detail akan diberikan saat pemesanan.</p>
                    
                    <h4>Fasilitas:</h4>
                    <ul class="package-facilities">
                        <li>Transportasi lokal</li>
                        <li>Penginapan 2 malam</li>
                        <li>Makan 3x sehari</li>
                        <li>Tiket masuk semua destinasi</li>
                        <li>Guide profesional</li>
                        <li>Workshop membatik</li>
                        <li>Peralatan outbound</li>
                        <li>Dokumentasi</li>
                        <li>Asuransi</li>
                        <li>Oleh-oleh khas</li>
                    </ul>
                    
                    <button class="close-package" onclick="closePackage()">Tutup</button>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Pariwisewu</h3>
                    <p>Menyediakan pengalaman wisata terbaik di Kabupaten Pringsewu dengan konsep 5A: Atraksi, Akomodasi, Aksesibilitas, Aktivitas, dan Amenitas. memastikan pengalaman menarik dan unik bagi pengunjung</p>
                    <div class="social-links">
                        <a href="https://instagram.com/pariwisewu" class="social-link" target="_blank">i</a>
                        <a href="https://wa.me/085839227740" class="social-link" target="_blank">w</a>
                        <a href="https://shorturl.at/UYCSU" class="social-link" target="_blank">P</a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Link Cepat</h3>
                    <ul>
                        <li><a href="#">Beranda</a></li>
                        <li><a href="#packages">Paket Wisata</a></li>
                        <li><a href="https://www.canva.com/design/DAGhWGsmz54/ndH4PIUD9CmvonmHxqqKgA/view?utm_content=DAGhWGsmz54&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h4b937c3105" target="_blank">Denah Wisata</a></li>
                        <li><a href="https://www.instagram.com/pariwisewu" target="_blank">Informasi UMKM</a></li>
                        <li><a href="https://wa.me/6281234567890" target="_blank">Kontak</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Kontak Kami</h3>
                    <ul>
                        <li>Jl. Wisata No. 123, Pringsewu, Lampung</li>
                        <li>0725-123456</li>
                        <li>info@wisatapringsewu.com</li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 Wisata Pringsewu. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        function toggleMenu() {
            document.getElementById('mainMenu').classList.toggle('active');
        }
        
        function showPackage(packageId) {
            // Hide all package details first
            let packageDetails = document.querySelectorAll('.package-detail');
            packageDetails.forEach(function(detail) {
                detail.classList.remove('active');
            });
            
            // Show the selected package
            document.getElementById(packageId).classList.add('active');
            
            // Scroll to package details
            document.getElementById('packageDetails').scrollIntoView({behavior: 'smooth'});
        }
        
        function closePackage() {
            let packageDetails = document.querySelectorAll('.package-detail');
            packageDetails.forEach(function(detail) {
                detail.classList.remove('active');
            });
        }


        let images = document.querySelectorAll(".carousel img");
        let index = 0;

        function changeImage() {
            images[index].classList.remove("active");
            index = (index + 1) % images.length;
            images[index].classList.add("active");
        }

        setInterval(changeImage, 3000);

    </script>
    
</body>
</html>