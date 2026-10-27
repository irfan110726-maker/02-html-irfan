<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Mahasiswa</title>

    <!-- Menghubungkan file CSS eksternal -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <nav class="navbar">
            <h2 class="logo">MyPortfolio</h2>
            <ul>
                <li><a href="#beranda">Beranda</a></li>
                <li><a href="#tentang">Tentang</a></li>
                <li><a href="#proyek">Proyek</a></li>
                <li><a href="#kontak">Kontak</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="beranda" class="hero">
            <div class="hero-content">
                <p class="subtitle">SELAMAT DATANG DI PORTOFOLIO SAYA</p>
                <h1>Halo, Saya <span>irfan Mahasiswa Matematika</span></h1>
                <p>
                    Saya tertarik pada matematika, teknologi,
                    pemrograman, dan pengembangan website.
                </p>
                <a href="#proyek" class="btn">Lihat Proyek</a>
            </div>
        </section>

        <section id="tentang" class="section">
            <h2>Tentang Saya</h2>
            <p>
                Saya adalah mahasiswa yang senang belajar hal baru,
                mengembangkan keterampilan digital, dan memecahkan
                masalah melalui pemikiran logis.
            </p>
        </section>

        <section id="proyek" class="section projects">
            <h2>Proyek Saya</h2>

            <div class="project-container">
                <article class="project-card">
                    <h3>Website Profil</h3>
                    <p>
                        Website sederhana menggunakan HTML
                        dan CSS untuk menampilkan profil pribadi.
                    </p>
                </article>

                <article class="project-card">
                    <h3>Komputasi Statistika</h3>
                    <p>
                        Analisis data numerik menggunakan
                        Python dan visualisasi grafik.
                    </p>
                </article>

                <article class="project-card">
                    <h3>Formulir Pendaftaran</h3>
                    <p>
                        Membuat formulir pendaftaran mahasiswa
                        menggunakan HTML dan CSS.
                    </p>
                </article>
            </div>
        </section>

        <section id="kontak" class="section contact">
            <h2>Hubungi Saya</h2>
            <p>Terima kasih telah mengunjungi portofolio saya.</p>
            <a href="mailto:emailkamu@example.com" class="btn">
                Kirim Email
            </a>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 MyPortfolio. Dibuat dengan HTML dan CSS.</p>
    </footer>

</body>
</html>
* Pengaturan dasar */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.7;
    color: #243047;
    background-color: #f5f7fb;
}

/* Navigasi */
header {
    background-color: #172554;
    color: white;
}

.navbar {
    max-width: 1100px;
    margin: auto;
    padding: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}

.logo {
    color: #60a5fa;
    font-size: 25px;
}

.navbar ul {
    display: flex;
    list-style: none;
    gap: 22px;
    flex-wrap: wrap;
}

.navbar a {
    color: white;
    text-decoration: none;
    transition: color 0.3s;
}

.navbar a:hover {
    color: #60a5fa;
}

/* Bagian beranda */
.hero {
    min-height: 480px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 70px 20px;
    background: linear-gradient(135deg, #172554, #2563eb);
    color: white;
}

.hero-content {
    max-width: 750px;
}

.subtitle {
    color: #bfdbfe;
    letter-spacing: 2px;
    font-size: 13px;
    margin-bottom: 15px;
}

.hero h1 {
    font-size: 40px;
    line-height: 1.3;
    margin-bottom: 20px;
}

.hero h1 span {
    color: #93c5fd;
}

.hero p {
    margin-bottom: 25px;
}

/* Tombol */
.btn {
    display: inline-block;
    background-color: #60a5fa;
    color: #172554;
    padding: 11px 24px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.3s;
}

.btn:hover {
    background-color: #bfdbfe;
}

/* Bagian umum */
.section {
    max-width: 1100px;
    margin: auto;
    padding: 70px 20px;
    text-align: center;
}

.section h2 {
    color: #172554;
    font-size: 30px;
    margin-bottom: 20px;
}

.section > p {
    max-width: 750px;
    margin: auto;
}

/* Kartu proyek */
.projects {
    max-width: 1200px;
}

.project-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 22px;
    margin-top: 35px;
    text-align: left;
}

.project-card {
    background-color: white;
    padding: 28px;
    border-radius: 12px;
    border: 1px solid #e2e8f0;
    box-shadow: 0 5px 15px rgba(23, 37, 84, 0.06);
    transition: transform 0.3s, box-shadow 0.3s;
}

.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(23, 37, 84, 0.12);
}

.project-card h3 {
    color: #2563eb;
    margin-bottom: 12px;
}

/* Kontak */
.contact {
    background-color: #eaf1ff;
    max-width: 100%;
}

.contact .btn {
    margin-top: 20px;
}

/* Footer */
footer {
    background-color: #172554;
    color: white;
    text-align: center;
    padding: 22px 15px;
}

/* Tampilan HP dan tablet */
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
    }

    .navbar ul {
        justify-content: center;
        gap: 15px;
    }

    .hero h1 {
        font-size: 30px;
    }

    .project-container {
        grid-template-columns: 1fr;
    }

    .section {
        padding: 50px 20px;
    }
}
