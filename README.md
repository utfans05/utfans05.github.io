<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resume | Red Apple Crafting</title>
    <link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,700;1,400&family=Playfair+Display:ital,wght@0,600;0,800;1,600&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-cream: #fcfbf8;
            --crimson: #8a1c1c;
            --sage: #8f9c80;
            --text-dark: #2c2a25;
            --text-light: #5a574f;
            --font-heading: 'Playfair Display', serif;
            --font-body: 'Lora', serif;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: var(--bg-cream);
            color: var(--text-dark);
            font-family: var(--font-body);
            line-height: 1.6;
            background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100' height='100' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
        }

        h1, h2, h3, h4 {
            font-family: var(--font-heading);
            color: var(--crimson);
            margin-top: 0;
        }

        a {
            color: var(--sage);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        a:hover {
            color: var(--crimson);
        }

        /* Header Styling */
        header {
            text-align: center;
            padding: 40px 20px 20px;
            border-bottom: 2px dashed var(--sage);
            max-width: 1000px;
            margin: 0 auto;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 5px;
            letter-spacing: 1px;
        }

        header h2 {
            font-size: 1.2rem;
            color: var(--text-light);
            font-weight: 400;
            font-style: italic;
        }

        nav {
            margin-top: 20px;
        }

        nav a {
            margin: 0 15px;
            font-weight: 700;
            text-transform: uppercase;
            font-size: 0.9rem;
            letter-spacing: 1px;
        }

        /* Layout */
        .container {
            display: flex;
            max-width: 1000px;
            margin: 40px auto;
            gap: 40px;
            padding: 0 20px;
        }

        .sidebar {
            flex: 1;
            min-width: 250px;
            background: #ffffff;
            padding: 30px;
            border: 1px solid rgba(143, 156, 128, 0.3);
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.02);
            height: fit-content;
        }

        .main-content {
            flex: 2.5;
        }

        /* Sidebar Elements */
        .profile-img {
            width: 100%;
            border-radius: 50%;
            border: 3px solid var(--sage);
            margin-bottom: 20px;
        }

        .sidebar-section {
            margin-bottom: 30px;
        }

        .sidebar-section h3 {
            font-size: 1.2rem;
            border-bottom: 1px solid rgba(138, 28, 28, 0.2);
            padding-bottom: 5px;
            margin-bottom: 15px;
        }

        .floral-divider {
            text-align: center;
            color: var(--sage);
            margin: 15px 0;
            font-size: 1.2rem;
        }

        /* Main Content Elements */
        .section-title {
            font-size: 1.8rem;
            border-bottom: 2px solid var(--sage);
            padding-bottom: 10px;
            margin-bottom: 25px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .item {
            margin-bottom: 35px;
        }

        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            margin-bottom: 10px;
        }

        .item-header h3 {
            margin-bottom: 0;
            font-size: 1.4rem;
        }

        .item-meta {
            color: var(--text-light);
            font-style: italic;
            font-size: 0.95rem;
        }

        .item-subheader {
            font-weight: 700;
            color: var(--text-dark);
            margin-bottom: 15px;
        }

        ul {
            padding-left: 20px;
            color: var(--text-dark);
        }

        li {
            margin-bottom: 8px;
        }

        li::marker {
            color: var(--crimson);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .container {
                flex-direction: column;
            }
            nav a {
                display: inline-block;
                margin: 5px 10px;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>[Your Name]</h1>
        <h2>Artisanal Business Owner & Creator</h2>
        <nav>
            <a href="#experiences">Experiences</a>
            <a href="#education">Education</a>
            <a href="#skills">Skills</a>
            <a href="#interests">Interests</a>
        </nav>
    </header>

    <div class="container">
        <!-- Left Sidebar -->
        <aside class="sidebar">
            <img src="https://via.placeholder.com/300x300.png?text=Profile+Photo" alt="Profile" class="profile-img">
            
            <div class="sidebar-section">
                <h3>Location</h3>
                <p>United States</p>
            </div>

            <div class="sidebar-section">
                <h3>Links</h3>
                <p><a href="#">LinkedIn</a><br>
                   <a href="#">Portfolio</a></p>
            </div>

            <div class="floral-divider">❦</div>

            <div class="sidebar-section">
                <h3>About Me</h3>
                <p>I am a passionate creator dedicated to bringing whimsical and elegant designs to life. I specialize in curated, handmade goods and establishing cohesive brand identities rooted in natural beauty and rustic textures.</p>
            </div>
        </aside>

        <!-- Right Main Content -->
        <main class="main-content">
            
            <!-- Experiences -->
            <section id="experiences">
                <h2 class="section-title">Experiences</h2>
                
                <div class="item">
                    <div class="item-header">
                        <h3>Founder & Lead Creator</h3>
                        <span class="item-meta">2026 - Present</span>
                    </div>
                    <div class="item-subheader">Red Apple Crafting Company</div>
                    <ul>
                        <li>Develop and curate a line of artisanal, handmade goods with a focus on high-quality materials and rustic elegance.</li>
                        <li>Design and implement comprehensive brand identity, incorporating botanical motifs such as stylized apples, roses, and dandelions.</li>
                        <li>Manage daily business operations, e-commerce fulfillment, and customer relations to ensure exceptional service.</li>
                    </ul>
                </div>

                <div class="item">
                    <div class="item-header">
                        <h3>Previous Role Title</h3>
                        <span class="item-meta">Year - Year</span>
                    </div>
                    <div class="item-subheader">Company Name</div>
                    <ul>
                        <li>Describe your achievements and responsibilities here.</li>
                        <li>Use action verbs to highlight the impact you made.</li>
                    </ul>
                </div>
            </section>

            <!-- Education -->
            <section id="education">
                <h2 class="section-title">Education</h2>
                
                <div class="item">
                    <div class="item-header">
                        <h3>Degree Name</h3>
                        <span class="item-meta">Graduation Year</span>
                    </div>
                    <div class="item-subheader">University or Institution Name</div>
                    <p>Details about your studies, honors, or specific coursework relevant to your career path.</p>
                </div>
            </section>

            <!-- Skills -->
            <section id="skills">
                <h2 class="section-title">Skills</h2>
                <div style="display: flex; gap: 40px; flex-wrap: wrap;">
                    <div>
                        <h4 style="margin-bottom: 10px;">Design & Branding</h4>
                        <ul style="margin-top: 0;">
                            <li>Visual Identity</li>
                            <li>Typography Selection</li>
                            <li>Color Theory</li>
                        </ul>
                    </div>
                    <div>
                        <h4 style="margin-bottom: 10px;">Business Operations</h4>
                        <ul style="margin-top: 0;">
                            <li>E-commerce Management</li>
                            <li>Client Relations</li>
                            <li>Product Curation</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Interests -->
            <section id="interests">
                <h2 class="section-title">Interests</h2>
                <ul style="columns: 2;">
                    <li>Botanical Illustration</li>
                    <li>Papercrafting</li>
                    <li>Artisanal Markets</li>
                    <li>Sustainable Materials</li>
                </ul>
            </section>

        </main>
    </div>

</body>
</html>
