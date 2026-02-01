[index.html](https://github.com/user-attachments/files/24994325/index.html)
<!DOCTYPE html>
<html lang="pt-pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Michelle Tembe | Software Engineer</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;500&family=Montserrat:wght@200;400&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
</head>
<body>[style.css](https://github.com/user-attachments/files/24994326/style.css):root {
    --dark: #1a1a1a;
    --gold: #b5835a;
    --glass: rgba(255, 255, 255, 0.7);
}

* { margin: 0; padding: 0; box-sizing: border-box; }

body {
    font-family: 'Montserrat', sans-serif;
    color: var(--dark);
    display: flex;
    justify-content: center;
    overflow-x: hidden;
    min-height: 100vh;
}

/* FUNDO QUE MUDA DE COR (AURORA LUXURY) */
.animated-bg {
    position: fixed;
    top: 0; left: 0; width: 100%; height: 100%;
    background: linear-gradient(45deg, #f7ece9, #e8f0f2, #f4e9e2, #f7ece9);
    background-size: 400% 400%;
    animation: gradientMove 15s ease infinite;
    z-index: -1;
}

@keyframes gradientMove {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}

.container {
    max-width: 450px;
    width: 90%;
    padding: 60px 0;
    text-align: center;
}

/* Substituindo a foto por um selo de iniciais luxuoso */
.initials-circle {
    width: 80px; height: 80px;
    border: 1px solid var(--dark);
    border-radius: 50%;
    margin: 0 auto 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.5rem;
    letter-spacing: 3px;
}

.name {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2.8rem;
    font-weight: 500;
}

.divider {
    width: 40px; height: 1px;
    background: var(--dark);
    margin: 20px auto;
}

.role {
    font-size: 0.6rem;
    letter-spacing: 3px;
    line-height: 1.8;
    margin-bottom: 40px;
    opacity: 0.8;
}

.email-area { margin-bottom: 40px; }
.email-area p { font-size: 0.8rem; margin-bottom: 10px; font-weight: 300; }
.email-text { text-decoration: none; color: var(--dark); font-weight: 400; }

/* BOTÕES INTERATIVOS */
.links-grid { display: flex; flex-direction: column; gap: 15px; }

.luxury-btn {
    background: var(--glass);
    backdrop-filter: blur(5px);
    padding: 22px;
    text-decoration: none;
    color: var(--dark);
    font-size: 0.75rem;
    letter-spacing: 2px;
    border: 1px solid rgba(255,255,255,0.4);
    transition: all 0.4s ease;
}

.luxury-btn:hover {
    background: var(--dark);
    color: white;
    transform: scale(1.02);
}

footer { margin-top: 60px; font-size: 0.5rem; letter-spacing: 3px; opacity: 0.4; }


    <div class="animated-bg"></div>

    <div class="container" data-aos="fade-up" data-aos-duration="1500">
        <header>
            <div class="initials-circle">MT</div>
            <h1 class="name">Michelle Tembe</h1>
            <div class="divider"></div>
            <p class="role">COMPUTER ENGINEERING STUDENT | SOFTWARE & CLOUD</p>
        </header>

        <section class="email-area">
            <p>Find all my links here!</p>
            <a href="mailto:michellesonio703@gmail.com" class="email-text">📩 michellesonio703@gmail.com</a>
        </section>

        <nav class="links-grid">
            <a href="https://www.linkedin.com/in/michelle-tembe" target="_blank" class="luxury-btn">LINKEDIN</a>
            <a href="https://github.com/michelle-tembe" target="_blank" class="luxury-btn">GITHUB</a>
            <a href="https://www.instagram.com/_michelle_tembe" target="_blank" class="luxury-btn">INSTAGRAM</a>
        </nav>

        <footer>
            <p>BASED IN MOZAMBIQUE • DIGITAL SOLUTIONS</p>
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ once: true });</script>
</body>
</html>
