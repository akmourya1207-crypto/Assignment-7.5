Here is your complete Assignment 7.5 — Flexbox Mini-Project. This project includes all five required sections: a navigation bar, hero section, three feature cards, a call-to-action section, and a footer.

The page uses Flexbox throughout, consistent colors and spacing, and responsive CSS so the content fits on desktop, tablet, and mobile screens.

I'll provide the complete working HTML/CSS code first, followed by instructions for creating the separate files and uploading your project to GitHub.
1. Create the project files
Create a folder named Assignment-7.5 with these two files:
index.html

Contains the webpage structure and content.



style.css

Contains the Flexbox layout, colors, spacing, and responsive styles.



2. HTML code — index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A responsive landing page built with HTML and CSS Flexbox.">
    <title>FlexStart - Assignment 7.5</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation Bar -->
    <header class="site-header">
        <nav class="navbar container">
            <a href="#home" class="logo">Flex<span>Start</span></a>

            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

            <a href="#contact" class="btn nav-btn">Get Started</a>
        </nav>
    </header>

    <main>
        <!-- Hero Section -->
        <section class="hero container" id="home">
            <div class="hero-content">
                <span class="eyebrow">WELCOME TO FLEXSTART</span>

                <h1>Build Something <span>Amazing.</span></h1>

                <p>
                    Turn your ideas into beautiful digital experiences.
                    Discover a simple, modern, and responsive way to
                    present your business or personal project online.
                </p>

                <div class="hero-actions">
                    <a href="#features" class="btn">Explore Features &rarr;</a>
                    <a href="#about" class="btn btn-outline">Learn More</a>
                </div>

                <p class="hero-note">
                    Designed for desktop, tablet, and mobile.
                </p>
            </div>

            <div class="hero-visual" aria-label="Creative web design illustration">
                <div class="visual-circle circle-one"></div>
                <div class="visual-circle circle-two"></div>

                <div class="browser-card">
                    <div class="browser-top">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>

                    <div class="browser-content">
                        <div class="mock-sidebar"></div>
                        <div class="mock-main">
                            <div class="mock-heading"></div>
                            <div class="mock-line"></div>
                            <div class="mock-line short"></div>

                            <div class="mock-cards">
                                <div></div>
                                <div></div>
                            </div>
                        </div>
                    </div>

                    <div class="visual-caption">
                        <span class="caption-icon">&lt;/&gt;</span>
                        <div>
                            <strong>Creative Design</strong>
                            <p>Design. Develop. Deliver.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Features Section -->
        <section class="features-section" id="features">
            <div class="container">
                <div class="section-heading">
                    <span class="eyebrow">OUR FEATURES</span>
                    <h2>Everything You Need</h2>
                    <p>
                        Powerful ideas, simple design, and a great
                        experience on every screen.
                    </p>
                </div>

                <div class="feature-container">
                    <article class="feature-card">
                        <div class="feature-icon icon-blue">✦</div>
                        <h3>Modern Design</h3>
                        <p>
                            Enjoy a clean and attractive interface
                            with consistent colors, typography,
                            and comfortable spacing.
                        </p>
                        <a href="#about" class="feature-link">
                            Learn more &rarr;
                        </a>
                    </article>

                    <article class="feature-card">
                        <div class="feature-icon icon-purple">▣</div>
                        <h3>Fully Responsive</h3>
                        <p>
                            Flexbox and media queries help the
                            layout adapt to desktops, tablets,
                            and smaller mobile screens.
                        </p>
                        <a href="#about" class="feature-link">
                            Learn more &rarr;
                        </a>
                    </article>

                    <article class="feature-card">
                        <div class="feature-icon icon-green">⚡</div>
                        <h3>Easy to Use</h3>
                        <p>
                            Clear navigation and well-organized
                            content make the website simple
                            for visitors to explore.
                        </p>
                        <a href="#about" class="feature-link">
                            Learn more &rarr;
                        </a>
                    </article>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section class="about-section container" id="about">
            <div class="about-content">
                <span class="eyebrow">ABOUT THIS PROJECT</span>
                <h2>Built with HTML and CSS Flexbox</h2>
                <p>
                    This mini-project demonstrates how Flexbox can
                    organize navigation links, align hero content,
                    and arrange feature cards into a responsive layout.
                    The page uses reusable CSS classes and media
                    queries to maintain a consistent design.
                </p>
            </div>

            <div class="about-points">
                <p>✓ Flexible layouts</p>
                <p>✓ Consistent spacing</p>
                <p>✓ Mobile-friendly design</p>
            </div>
        </section>

        <!-- Call-to-Action Section -->
        <section class="cta-section" id="contact">
            <div class="container cta-content">
                <div>
                    <h2>Ready to Get Started?</h2>
                    <p>
                        Take the next step and turn your idea into
                        something amazing.
                    </p>
                </div>

                <a href="mailto:student@example.com" class="btn cta-btn">
                    Contact Us &rarr;
                </a>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="site-footer">
        <div class="container footer-content">
            <p>&copy; 2026 FlexStart. Assignment 7.5.</p>
            <p>Created using HTML and CSS Flexbox.</p>
        </div>
    </footer>

</body>
</html>



3. CSS code — style.css

/* Assignment 7.5 - Flexbox Mini-Project */

/* 1. Reset and common styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 85px;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    color: #26344b;
    background-color: #ffffff;
    line-height: 1.7;
    overflow-wrap: break-word;
}

a {
    text-decoration: none;
}

.container {
    width: 100%;
    max-width: 1160px;
    margin: 0 auto;
    padding-left: 24px;
    padding-right: 24px;
}

.btn {
    display: inline-block;
    padding: 12px 22px;
    border: 2px solid #3264df;
    border-radius: 8px;
    background-color: #3264df;
    color: #ffffff;
    font-size: 15px;
    font-weight: bold;
    text-align: center;
    transition: background-color 0.3s, transform 0.3s;
}

.btn:hover {
    background-color: #2049b8;
    border-color: #2049b8;
    transform: translateY(-2px);
}

.eyebrow {
    display: inline-block;
    margin-bottom: 12px;
    color: #3264df;
    font-size: 12px;
    font-weight: bold;
    letter-spacing: 2px;
}

/* 2. Navigation Bar - Flexbox */
.site-header {
    position: sticky;
    top: 0;
    z-index: 100;
    background-color: #ffffff;
    border-bottom: 1px solid #e8edf5;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 24px;
    min-height: 78px;
}

.logo {
    color: #1b2d4b;
    font-size: 27px;
    font-weight: bold;
    white-space: nowrap;
}

.logo span {
    color: #3264df;
}

.nav-links {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 28px;
    list-style: none;
}

.nav-links a {
    color: #536179;
    font-size: 15px;
    transition: color 0.3s;
}

.nav-links a:hover {
    color: #3264df;
}

.nav-btn {
    white-space: nowrap;
}

/* 3. Hero Section - Side-by-side Flexbox */
.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 55px;
    padding-top: 75px;
    padding-bottom: 85px;
}

.hero-content {
    flex: 1 1 50%;
    min-width: 0;
}

.hero-content h1 {
    max-width: 540px;
    margin-bottom: 22px;
    color: #1b2d4b;
    font-size: clamp(36px, 5vw, 58px);
    line-height: 1.15;
    letter-spacing: -1.5px;
}

.hero-content h1 span {
    color: #3264df;
}

.hero-content > p:not(.hero-note) {
    max-width: 520px;
    margin-bottom: 26px;
    color: #65728a;
    font-size: 17px;
}

.hero-actions {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 14px;
    margin-bottom: 20px;
}

.btn-outline {
    background-color: #ffffff;
    color: #3264df;
}

.btn-outline:hover {
    background-color: #edf2ff;
    color: #2049b8;
}

.hero-note {
    color: #758197;
    font-size: 13px;
}

/* 4. CSS illustration */
.hero-visual {
    position: relative;
    flex: 1 1 50%;
    min-width: 0;
    min-height: 370px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #edf2ff, #f5efff);
    border-radius: 45% 55% 50% 40%;
    padding: 35px;
}

.visual-circle {
    position: absolute;
    border-radius: 50%;
}

.circle-one {
    top: 10%;
    right: 8%;
    width: 65px;
    height: 65px;
    background-color: #d5e2ff;
}

.circle-two {
    bottom: 8%;
    left: 7%;
    width: 45px;
    height: 45px;
    background-color: #c7f4df;
}

.browser-card {
    position: relative;
    z-index: 1;
    width: 100%;
    max-width: 410px;
    background-color: #ffffff;
    border: 1px solid #e1e7f1;
    border-radius: 14px;
    overflow: hidden;
    box-shadow: 0 18px 45px #273d7018;
}

.browser-top {
    display: flex;
    align-items: center;
    gap: 6px;
    padding: 13px;
    border-bottom: 1px solid #e8edf5;
}

.browser-top span {
    width: 9px;
    height: 9px;
    border-radius: 50%;
    background-color: #f4a5a5;
}

.browser-top span:nth-child(2) {
    background-color: #f5d276;
}

.browser-top span:nth-child(3) {
    background-color: #7bd6a7;
}

.browser-content {
    display: flex;
    gap: 15px;
    min-height: 180px;
    padding: 22px 16px;
}

.mock-sidebar {
    flex: 0 0 23%;
    border-radius: 7px;
    background-color: #e9efff;
}

.mock-main {
    flex: 1;
    min-width: 0;
}

.mock-heading {
    width: 75%;
    height: 16px;
    margin-bottom: 15px;
    border-radius: 5px;
    background-color: #3264df;
}

.mock-line {
    width: 100%;
    height: 8px;
    margin-bottom: 9px;
    border-radius: 5px;
    background-color: #e2e8f3;
}

.mock-line.short {
    width: 65%;
}

.mock-cards {
    display: flex;
    gap: 10px;
    margin-top: 22px;
}

.mock-cards div {
    flex: 1;
    height: 55px;
    border-radius: 7px;
    background-color: #e5f6ed;
}

.mock-cards div:last-child {
    background-color: #f0e9ff;
}

.visual-caption {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 15px;
    border-top: 1px solid #e8edf5;
}

.caption-icon {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 43px;
    height: 43px;
    flex-shrink: 0;
    border-radius: 10px;
    background-color: #3264df;
    color: white;
    font-weight: bold;
}

.visual-caption strong {
    color: #1b2d4b;
}

.visual-caption p {
    color: #758197;
    font-size: 13px;
}

/* 5. Features Section */
.features-section {
    padding-top: 75px;
    padding-bottom: 85px;
    background-color: #f6f8fc;
}

.section-heading {
    margin-bottom: 40px;
    text-align: center;
}

.section-heading h2,
.about-content h2 {
    color: #1b2d4b;
    font-size: 34px;
    line-height: 1.3;
    margin-bottom: 12px;
}

.section-heading > p {
    color: #65728a;
}

/* Responsive row of three feature cards */
.feature-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 24px;
}

.feature-card {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    flex: 1 1 280px;
    min-width: 0;
    max-width: 360px;
    padding: 28px;
    background-color: #ffffff;
    border: 1px solid #e5eaf3;
    border-radius: 12px;
    box-shadow: 0 5px 20px #1b2d4b08;
    transition: transform 0.3s, box-shadow 0.3s;
}

.feature-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 25px #1b2d4b12;
}

.feature-icon {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 52px;
    height: 52px;
    margin-bottom: 20px;
    border-radius: 12px;
    font-size: 25px;
}

.icon-blue {
    color: #3264df;
    background-color: #e8efff;
}

.icon-purple {
    color: #8055d9;
    background-color: #f0eaff;
}

.icon-green {
    color: #159b62;
    background-color: #e3f8ed;
}

.feature-card h3 {
    margin-bottom: 10px;
    color: #1b2d4b;
    font-size: 20px;
}

.feature-card p {
    flex-grow: 1;
    margin-bottom: 18px;
    color: #65728a;
    font-size: 15px;
}

.feature-link {
    color: #3264df;
    font-weight: bold;
    font-size: 14px;
}

/* 6. About Section */
.about-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 35px;
    padding-top: 75px;
    padding-bottom: 75px;
}

.about-content {
    flex: 1 1 400px;
    min-width: 0;
}

.about-content h2 {
    font-size: 30px;
}

.about-content p {
    color: #65728a;
}

.about-points {
    display: flex;
    flex-direction: column;
    gap: 12px;
    flex: 0 1 280px;
    padding: 25px;
    background-color: #f6f8fc;
    border-radius: 12px;
}

.about-points p {
    color: #3264df;
    font-weight: bold;
}

/* 7. Call-to-Action Section */
.cta-section {
    background: linear-gradient(120deg, #244db5, #3264df);
    color: #ffffff;
}

.cta-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 25px;
    padding-top: 45px;
    padding-bottom: 45px;
}

.cta-content h2 {
    margin-bottom: 8px;
    font-size: 30px;
}

.cta-content p {
    color: #e1e9ff;
}

.cta-btn {
    flex-shrink: 0;
    background-color: #ffffff;
    color: #244db5;
    border-color: #ffffff;
}

.cta-btn:hover {
    background-color: #edf2ff;
    color: #173b91;
    border-color: #edf2ff;
}

/* 8. Footer */
.site-footer {
    background-color: #172744;
    color: #ffffff;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 12px;
    padding-top: 22px;
    padding-bottom: 22px;
}

.footer-content p {
    color: #c6d0e1;
    font-size: 13px;
}

/* 9. Tablet layout */
@media (max-width: 900px) {
    .navbar {
        flex-wrap: wrap;
        justify-content: center;
        padding-top: 16px;
        padding-bottom: 16px;
    }

    .logo {
        margin-right: auto;
    }

    .nav-links {
        gap: 16px;
    }

    .hero {
        gap: 30px;
        padding-top: 55px;
        padding-bottom: 60px;
    }

    .hero-visual {
        min-height: 320px;
        padding: 20px;
    }

    .feature-card {
        flex-basis: 240px;
    }
}

/* 10. Mobile layout */
@media (max-width: 650px) {
    .container {
        padding-left: 18px;
        padding-right: 18px;
    }

    .navbar {
        justify-content: center;
        gap: 14px;
    }

    .logo {
        width: 100%;
        margin-right: 0;
        text-align: center;
    }

    .nav-links {
        justify-content: center;
        gap: 12px 18px;
    }

    .nav-links a {
        font-size: 14px;
    }

    .nav-btn {
        padding: 9px 15px;
    }

    .hero {
        flex-direction: column;
        align-items: stretch;
        gap: 35px;
        padding-top: 45px;
        padding-bottom: 50px;
    }

    .hero-content {
        width: 100%;
    }

    .hero-content h1 {
        font-size: clamp(34px, 9vw, 46px);
        letter-spacing: -0.8px;
    }

    .hero-content > p:not(.hero-note) {
        font-size: 15px;
    }

    .hero-visual {
        width: 100%;
        min-height: 280px;
        padding: 18px;
    }

    .browser-content {
        min-height: 145px;
    }

    .features-section {
        padding-top: 55px;
        padding-bottom: 55px;
    }

    .section-heading h2 {
        font-size: 28px;
    }

    .feature-container {
        flex-direction: column;
        align-items: stretch;
    }

    .feature-card {
        flex: 1 1 auto;
        width: 100%;
        max-width: none;
    }

    .about-section {
        flex-direction: column;
        align-items: stretch;
        padding-top: 55px;
        padding-bottom: 55px;
    }

    .about-content h2 {
        font-size: 27px;
    }

    .cta-content {
        flex-direction: column;
        align-items: flex-start;
        padding-top: 35px;
        padding-bottom: 35px;
    }

    .cta-content h2 {
        font-size: 26px;
    }

    .footer-content {
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
}

/* Very narrow phones */
@media (max-width: 360px) {
    .hero-actions {
        flex-direction: column;
        align-items: stretch;
    }

    .hero-actions .btn {
        width: 100%;
    }

    .nav-links {
        gap: 10px;
    }

    .nav-links a {
        font-size: 13px;
    }

    .hero-visual {
        min-height: 240px;
        padding: 12px;
    }

    .visual-caption {
        padding: 10px;
    }
}



4. How your landing page meets the requirements
Requirement	Completed implementation
Navigation bar	Logo, links, and CTA button using Flexbox
Hero section	Heading, paragraph, buttons, and CSS illustration
Three feature cards	Modern Design, Fully Responsive, Easy to Use
CTA section	“Ready to Get Started?” with Contact Us button
Footer	Copyright and project information
gap	Adds spacing between navigation links, cards, and content
justify-content	Distributes and centers items
align-items	Aligns items vertically or across the cross-axis
flex-wrap	Allows content to move onto new rows
Responsive layout	Media queries for tablets, phones, and narrow screens
Overflow prevention	Flexible widths, min-width: 0, and responsive sizing

5. Run and test the project
1. Open Visual Studio Code or Notepad.
2. Create a folder named Assignment-7.5.
3. Save the HTML code as index.html.
4. Save the CSS code as style.css in the same folder.
5. Open index.html in Chrome.
6. Resize the browser to check desktop, tablet, and mobile layouts.
Take screenshots using Win + Shift + S:
- Assignment-7.5-Desktop.png — full page at desktop width.
- Assignment-7.5-Mobile.png — page at mobile width.
6. Upload your project to GitHub
Your assignment asks for a GitHub repository link. You can create one using these steps.
1. Open GitHub — Create a new repository and sign in.
2. Set the repository name to Assignment-7.5-Flexbox-Mini-Project and choose Public if your instructor needs to access it.
3. Click Create repository.
4. Use Add file → Upload files to upload index.html, style.css, and your screenshots. Click Commit changes.
5. To publish the webpage, open the repository's Settings → Pages, choose the main branch and / (root) folder, and save.
Your links will look like this after you create the repository:
- Repository: https://github.com/YOUR-USERNAME/Assignment-7.5-Flexbox-Mini-Project
- Live webpage: https://YOUR-USERNAME.github.io/Assignment-7.5-Flexbox-Mini-Project/
Replace YOUR-USERNAME with your actual GitHub username. These are URL patterns, not links to a repository already created for you.
Final submission checklist
- [ ] index.html
- [ ] style.css
- [ ] Assignment-7.5-Desktop.png
- [ ] Assignment-7.5-Mobile.png
- [ ] GitHub repository URL
Important: The project code is complete, but you still need to create the files, capture your screenshots, and upload them to GitHub before submitting.