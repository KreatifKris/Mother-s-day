# Mother-s-day


<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Hari Ibu, Mama!</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Montserrat:wght@300;500&display=swap" rel="stylesheet">
    <style>
        /* CSS DALAM SATU FILE */
        :root {
            --pink-soft: #ffafbd;
            --pink-warm: #ffc3a0;
            --text-color: #5a5a5a;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #fffafb;
            margin: 0;
            padding: 0;
            color: var(--text-color);
            overflow-x: hidden;
        }

        header {
            text-align: center;
            padding: 80px 20px;
            background: linear-gradient(135deg, var(--pink-soft), var(--pink-warm));
            color: white;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0% 100%);
        }

        header h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 4rem;
            margin: 0;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }

        header p {
            font-size: 1.2rem;
            font-weight: 300;
            margin-top: 10px;
        }

        /* Container Album */
        .album-wrapper {
            max-width: 1100px;
            margin: -50px auto 50px auto;
            padding: 20px;
        }

        .grid-album {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        /* Kartu Foto Ala Polaroid */
        .polaroid {
            background: white;
            padding: 15px 15px 30px 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.08);
            border-radius: 2px;
            transition: transform 0.4s ease;
            position: relative;
        }

        .polaroid:hover {
            transform: translateY(-10px) rotate(2deg);
            box-shadow: 0 15px 35px rgba(0,0,0,0.15);
        }

        .polaroid img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            filter: sepia(10%); /* Memberikan kesan vintage hangat */
        }

        .caption {
            font-family: 'Dancing Script', cursive;
            font-size: 1.4rem;
            text-align: center;
            margin-top: 15px;
            color: #d88a8a;
        }

        /* Pesan Penutup */
        .personal-note {
            text-align: center;
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            line-height: 1.8;
            font-style: italic;
            border-top: 1px solid #eee;
        }

        footer {
            text-align: center;
            padding: 30px;
            font-size: 0.8rem;
            background: #fdf2f4;
        }

        /* Responsive Mobile */
        @media (max-width: 600px) {
            header h1 { font-size: 2.5rem; }
            .album-wrapper { margin-top: 20px; }
        }
    </style>
</head>
<body>

    <header>
        <h1>Happy Mother's Day</h1>
        <p>Terima kasih telah menjadi pelangi di setiap hariku, Ma.</p>
    </header>

    <div class="album-wrapper">
        <div class="grid-album">
            
            <div class="polaroid">
                <img src="IMG_0708.jpeg" alt="Mama">
                <div class="caption">Mama harus terus sehat dan bahagia. Kami semua sayang mama dalam kondisi apapun.</div>
            </div>

            <div class="polaroid">
                <img src="IMG_0709.jpeg" alt="Mama">
                <div class="caption">Momen bahagia kita</div>
            </div>

            <div class="polaroid">
                <img src="IMG_0710.jpeg" alt="Mama">
                <div class="caption">Sehat selalu ya, Ma.... pokoknya harus terus ada sampai aku tuaaa</div>
            </div>

            <div class="polaroid">
                <img src="IMG_0712.jpeg" alt="Mama">
                <div class="caption">Terima kasih maa.., mama selalu ada buatku meski kadangkala diriku membuat amarah tongkat dewa😔</div>
            </div>

        </div>
    </div>

    <section class="personal-note">
        "mama adalah degup jantung di dalam rumah, dan tanpa mama, tidak ada detak jantung." <br>
        <strong>- I love you mom. kalau mama berdoa selalu namaku disebut, aku juga ma sellau menyebut mama dalam doa.</strong>
    </section>

    <footer>
        &copy; 2025 - Dibuat spesial untuk Hari Ibu
    </footer>

</body>

