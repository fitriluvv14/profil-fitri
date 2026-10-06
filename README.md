<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Profil Murid RPL</title>

    <!-- Bootstrap 5 -->
    <link href="" rel="stylesheet">

    <!-- Bootstrap Icons -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">

    <style>
        html {
            scroll-behavior: smooth;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            color: #222;
        }

        /* NAVBAR */
        .navbar {
            background: #111827;
            box-shadow: 0 2px 10px rgba(0,0,0,.2);
        }

        .navbar-brand {
            letter-spacing: 1px;
        }

        .nav-link {
            margin-left: 10px;
        }

        .nav-link:hover {
            color: #60a5fa !important;
        }

        /* HERO */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            background: linear-gradient(135deg,#111827,#1e3a8a);
            color: white;
            padding-top: 80px;
        }

        .hero h1 {
            font-size: 50px;
            font-weight: bold;
        }

        .hero h1 span {
            color: #60a5fa;
        }

        .hero p {
            line-height: 1.8;
        }

        .hero .btn {
            margin-right: 10px;
            margin-top: 10px;
        }

        /* PROFIL */
        .profile-circle {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            margin: auto;
            display: flex;
            justify-content: center;
            align-items: center;
            background: white;
            color: #1e3a8a;
            border: 10px solid #60a5fa;
            font-size: 120px;
        }

        /* SECTION */
        .section {
            padding: 90px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-weight: bold;
            font-size: 36px;
        }

        .section-title p {
            color: #666;
        }

        /* CARD */
        .custom-card {
            border: none;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,.08);
            transition: .3s;
        }

        .custom-card:hover {
            transform: translateY(-5px);
        }

        .custom-card h4 {
            color: #1e3a8a;
        }

        /* PROGRESS */
        .progress {
            height: 12px;
            border-radius: 20px;
        }

        .progress-bar {
            background: #2563eb;
        }

        /* JURUSAN */
        .nav-pills .nav-link {
            color: #1e3a8a;
            border-radius: 25px;
            padding: 10px 20px;
        }

        .nav-pills .nav-link.active {
            background: #1e3a8a;
            color: white;
        }

        .jurusan-card {
            border: none;
            border-radius: 20px;
            box-shadow: 0 5px 20px rgba(0,0,0,.08);
            min-height: 350px;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .jurusan-card h3 {
            margin-top: 20px;
            color: #1e3a8a;
        }

        .jurusan-card p {
            max-width: 750px;
            margin: 15px auto;
            line-height: 1.7;
        }

        /* LOGO */
        .logo-jurusan {
            width: 120px;
            height: 120px;
            object-fit: contain;
            margin-bottom: 10px;
        }

        /* MAP */
        .map-container {
            width: 100%;
            height: 450px;
            overflow: hidden;
            border-radius: 15px;
        }

        .map-container iframe {
            width: 100%;
            height: 100%;
            border: 0;
        }

        /* FOOTER */
        footer {
            background: #111827;
            color: white;
            text-align: center;
            padding: 40px 0;
        }

        footer h5 {
            font-weight: bold;
        }

        footer p {
            color: #d1d5db;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            .hero {
                text-align: center;
                padding-top: 120px;
                padding-bottom: 60px;
            }

            .hero h1 {
                font-size: 38px;
            }

            .profile-circle {
                width: 190px;
                height: 190px;
                font-size: 90px;
            }

            .section {
                padding: 70px 15px;
            }

            .nav-pills {
                gap: 8px;
            }

            .nav-pills .nav-link {
                padding: 8px 14px;
            }

            .map-container {
                height: 300px;
            }
        }
    </style>
</head>

<body data-bs-spy="scroll" data-bs-target="#navbar">

<!-- ================= NAVBAR ================= -->
<nav id="navbar" class="navbar navbar-expand-lg navbar-dark fixed-top">

    <div class="container">

        <a class="navbar-brand fw-bold" href="#beranda">
            <i class="bi bi-person-circle"></i>
            PROFIL MURID
        </a>

        <button class="navbar-toggler"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#menu">

            <span class="navbar-toggler-icon"></span>

        </button>

        <div class="collapse navbar-collapse" id="menu">

            <ul class="navbar-nav ms-auto">

                <li class="nav-item">
                    <a class="nav-link" href="#beranda">
                        Beranda
                    </a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#tentang">
                        Tentang Saya
                    </a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#jurusan">
                        Jurusan
                    </a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#denah">
                        Denah
                    </a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="#kontak">
                        Kontak
                    </a>
                </li>

            </ul>

        </div>

    </div>

</nav>


<!-- ================= BERANDA ================= -->
<section id="beranda" class="hero">

    <div class="container">

        <div class="row align-items-center">

            <div class="col-md-7">

                <p class="text-uppercase fw-bold">
                    Selamat Datang
                </p>

                <h1>
                    Halo, Saya
                    <span>Syah Fitri Balqis</span>
                </h1>

                <h4 class="mb-3">
                    Siswa Rekayasa Perangkat Lunak
                </h4>

                <p>
                    Saya adalah siswa SMK yang sedang belajar
                    mengembangkan kemampuan di bidang teknologi,
                    pemrograman, dan pengembangan website.
                </p>

                <a href="#tentang"
                   class="btn btn-primary">
                    Tentang Saya
                </a>

                <a href="#jurusan"
                   class="btn btn-outline-light">
                    Lihat Jurusan
                </a>

            </div>

            <div class="col-md-5 text-center mt-4 mt-md-0">

                <div class="profile-circle">
<img
src="Screenshot_2026-07-10-07-30-41-11.jpg" alt="foto profil Fitri">
                    <i class="bi bi-person-fill"></i>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- ================= TENTANG ================= -->
<section id="tentang" class="section">

    <div class="container">

        <div class="section-title">

            <h2>Tentang Saya</h2>

            <p>
                Informasi singkat mengenai diri saya
            </p>

        </div>

        <div class="row g-4">

            <!-- DATA DIRI -->
            <div class="col-md-6">

                <div class="card custom-card h-100">

                    <div class="card-body">

                        <h4>
                            <i class="bi bi-person-vcard"></i>
                            Data Diri
                        </h4>

                        <hr>

                        <p>
                            <strong>Nama:</strong>
                            Syah Fitri Balqis 
                        </p>

                        <p>
                            <strong>Kelas:</strong>
                            XI RPL
                        </p>

                        <p>
                            <strong>NIS:</strong>
                            14523
                        </p>

                        <p>
                            <strong>Jurusan:</strong>
                            Rekayasa Perangkat Lunak
                        </p>

                        <p>
                            <strong>Alamat:</strong>
                            Jl. mencirim prmh. persada suka maju No. 3
                        </p>

                    </div>

                </div>

            </div>


            <!-- KEAHLIAN -->
            <div class="col-md-6">

                <div class="card custom-card h-100">

                    <div class="card-body">

                        <h4>
                            <i class="bi bi-code-slash"></i>
                            Keahlian
                        </h4>

                        <hr>

                        <p>HTML / CSS</p>

                        <div class="progress mb-3">
                            <div class="progress-bar"
                                 style="width:85%">
                                85%
                            </div>
                        </div>

                        <p>JavaScript</p>

                        <div class="progress mb-3">
                            <div class="progress-bar"
                                 style="width:70%">
                                70%
                            </div>
                        </div>

                        <p>PHP & MySQL</p>

                        <div class="progress mb-3">
                            <div class="progress-bar"
                                 style="width:75%">
                                75%
                            </div>
                        </div>

                        <p>Git</p>

                        <div class="progress">
                            <div class="progress-bar"
                                 style="width:65%">
                                65%
                            </div>
                        </div>

                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- ================= JURUSAN ================= -->
<section id="jurusan"
         class="section bg-light">

    <div class="container">

        <div class="section-title">

            <h2>6 Jurusan di Sekolah</h2>

            <p>
                Kenali berbagai jurusan yang tersedia
            </p>

        </div>


        <!-- PILLS -->

        <ul class="nav nav-pills justify-content-center mb-4">

            <li class="nav-item">
                <button class="nav-link active"
                        data-bs-toggle="pill"
                        data-bs-target="#rpl">
                    RPL
                </button>
            </li>

            <li class="nav-item">
                <button class="nav-link"
                        data-bs-toggle="pill"
                        data-bs-target="#dkv">
                    DKV
                </button>
            </li>

            <li class="nav-item">
                <button class="nav-link"
                        data-bs-toggle="pill"
                        data-bs-target="#peksos">
                    PEKSOS
                </button>
            </li>

            <li class="nav-item">
                <button class="nav-link"
                        data-bs-toggle="pill"
                        data-bs-target="#tkj">
                    TKJ
                </button>
            </li>

            <li class="nav-item">
                <button class="nav-link"
                        data-bs-toggle="pill"
                        data-bs-target="#animasi">
                    ANIMASI
                </button>
            </li>

            <li class="nav-item">
                <button class="nav-link"
                        data-bs-toggle="pill"
                        data-bs-target="#pspt">
                    PSPT
                </button>
            </li>

        </ul>


        <!-- ISI JURUSAN -->

        <div class="tab-content">


            <!-- RPL -->

            <div class="tab-pane fade show active"
                 id="rpl">

                <div class="card jurusan-card">

                    <div class="card-body text-center">

                        <img src="IMG-20261006-WA0004.jpg"
                             class="logo-jurusan"
                             alt="Logo RPL">

                        <h3>
                            Rekayasa Perangkat Lunak
                        </h3>

                        <p>
                            <strong>Visi:</strong>
                            Pengembang perangkat lunak
                            kompeten dan kreatif.
                        </p>

                        <p>
                            <strong>Misi:</strong>
                            Mengembangkan kemampuan pemrograman,
                            teknologi, kreativitas, dan pemecahan masalah.
                        </p>

                    </div>

                </div>

            </div>


            <!-- DKV -->

            <div class="tab-pane fade"
                 id="dkv">

                <div class="card jurusan-card">

                    <div class="card-body text-center">

                        <img src="IMG-20261006-WA0003.jpg"
                             class="logo-jurusan"
                             alt="Logo DKV">

                        <h3>
                            Desain Komunikasi Visual
                        </h3>

                        <p>
                            <strong>Visi:</strong>
                            Desainer visual kreatif
                            untuk industri kreatif.
                        </p>

                        <p>
                            <strong>Misi:</strong>
                            Mengembangkan kreativitas dan kemampuan
                            menghasilkan karya visual.
                        </p>

                    </div>

                </div>

            </div>


            <!-- PEKSOS -->

            <div class="tab-pane fade"
                 id="peksos">

                <div class="card jurusan-card">

                    <div class="card-body text-center">

                        <img src="IMG-20261006-WA0007.jpg"
                             class="logo-jurusan"
                             alt="Logo PEKSOS">

                        <h3>
                            Pekerjaan Sosial
                        </h3>

                        <p>
                            <strong>Visi:</strong>
                            Tenaga sosial profesional
                            yang peduli dan berempati.
                        </p>

                        <p>
                            <strong>Misi:</strong>
                            Membentuk tenaga sosial yang mampu
                            membantu dan memberikan pelayanan sosial.
                        </p>

                    </div>

                </div>

            </div>


            <!-- TKJ -->

            <div class="tab-pane fade"
                 id="tkj">

                <div class="card jurusan-card">

                    <div class="card-body text-center">

                        <img src="IMG-20261006-WA0006.jpg"
                             class="logo-jurusan"
                             alt="Logo TKJ">

                        <h3>
                            Teknik Komputer dan Jaringan
                        </h3>

                        <p>
                            <strong>Visi:</strong>
                            Teknisi dan administrator
                            jaringan yang handal.
                        </p>

                        <p>
                            <strong>Misi:</strong>
                            Mengembangkan kemampuan instalasi,
                            konfigurasi, dan pengelolaan jaringan.
                        </p>

                    </div>

                </div>

            </div>


            <!-- ANIMASI -->

            <div class="tab-pane fade"
                 id="animasi">

                <div class="card jurusan-card">

                    <div class="card-body text-center">

                        <img src="IMG-20261006-WA0002.jpg"
                             class="logo-jurusan"
                             alt="Logo Animasi">

                        <h3>
                            Animasi
                        </h3>

                        <p>
                            <strong>Visi:</strong>
                            Animator kreatif dan produktif.
                        </p>

                        <p>
                            <strong>Misi:</strong>
                            Mengembangkan kreativitas dan kemampuan
                            menghasilkan karya animasi berkualitas.
                        </p>

                    </div>

                </div>

            </div>


            <!-- PSPT -->

            <div class="tab-pane fade"
                 id="pspt">

                <div class="card jurusan-card">

                    <div class="card-body text-center">

                        <img src="IMG-20261006-WA0005.jpg"
                             class="logo-jurusan"
                             alt="Logo PSPT">

                        <h3>
                            Produksi Siaran Program Televisi
                        </h3>

                        <p>
                            <strong>Visi:</strong>
                            Insan pertelevisian profesional
                            dan beretika.
                        </p>

                        <p>
                            <strong>Misi:</strong>
                            Mengembangkan keterampilan produksi,
                            penyiaran, dan kreativitas di bidang televisi.
                        </p>

                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<section id="denah"
         class="section">

    <div class="container">

        <div class="section-title">

            <h2>Denah Sekolah</h2>

            <p>
                Rute dari rumah menuju sekolah
            </p>

        </div>

        <div class="card custom-card">

            <div class="card-body">

                <h4>
                    <i class="bi bi-geo-alt-fill"></i>
                    Lokasi Sekolah
                </h4>

                <p>
                    Tujuan:
                    <strong>
                        Jl. Patriot No. 20, Sunggal
                    </strong>
                </p>

                <div class="map-container">

                    <iframe
                        src="https://www.google.com/maps?q=Jl.%20Patriot%20No.%2020,%20Sunggal&output=embed"
                       
