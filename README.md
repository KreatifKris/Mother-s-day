# Mother-s-day



<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Hari Ibu, Mama!</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Montserrat:wght@300;500&display=swap" rel="stylesheet">
    <style>
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

        /* --- LAYER 1: OVERLAY PEMBUKA --- */
        #overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, var(--pink-soft), var(--pink-warm));
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            transition: opacity 1s ease, visibility 1s;
            color: white;
            text-align: center;
        }

        .heart-btn {
            font-size: 80px;
            cursor: pointer;
            animation: pulse 1.5s infinite;
            background: none;
            border: none;
            color: white;
            margin-bottom: 20px;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }

        /* --- LAYER 2: ISI KONTEN --- */
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

        .album-wrapper {
            max-width: 1100px;
            margin: -50px auto 50px auto;
            padding: 20px;
            opacity: 0; /* Awalnya sembunyi */
            transform: translateY(30px);
            transition: all 1.5s ease;
        }

        /* Munculkan konten saat overlay hilang */
        .show-content {
            opacity: 1 !important;
            transform: translateY(0) !important;
        }

        .grid-album {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .polaroid {
            background: white;
            padding: 15px 15px 30px 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.08);
            border-radius: 2px;
            transition: transform 0.4s ease;
        }

        .polaroid:hover {
            transform: translateY(-10px) rotate(2deg);
        }

        .polaroid img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            filter: sepia(10%);
        }

        .caption {
            font-family: 'Dancing Script', cursive;
            font-size: 1.4rem;
            text-align: center;
            margin-top: 15px;
            color: #d88a8a;
        }

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
    </style>
</head>
<body>

    <div id="overlay">
        <button class="heart-btn" onclick="bukaKado()">❤️</button>
        <h2>Ada kejutan buat Mama...<br><small>(Klik hatinya ya, Ma)</small></h2>
    </div>

    <header>
        <h1>Happy Mother's Day</h1>
        <p>Terima kasih telah menjadi pelangi di setiap hariku, Ma.</p>
    </header>

    <div class="album-wrapper" id="albumContent">
        <div class="grid-album">
            
            <div class="polaroid">
                <img src="IMG_0713.jpeg" alt="Mama">
                <div class="caption">Mama harus terus sehat dan bahagia. Kami semua sayang mama.</div>
            </div>

            <div class="polaroid">
                <img src="IMG_0709.jpeg" alt="Mama">
                <div class="caption">Mama selalu ada buatku, sedangkan orang lain belum tentu ada buatku</div>
            </div>

            <div class="polaroid">
                <img src="IMG_0710.jpeg" alt="Mama">
                <div class="caption">Sehat selalu ya, Ma... harus ada sampai aku tua!</div>
            </div>

            <div class="polaroid">
                <img src="IMG_0712.jpeg" alt="Mama">
                <div class="caption">Terima kasih Mama selalu sabar menghadapiku.</div>
            </div>

        </div>
    </div>

    <section class="personal-note">
        "Mama adalah degup jantung di dalam rumah, dan tanpa mama, tidak ada detak jantung." <br>
        <strong>- I love you mom</strong>
    </section>

    <footer>
        &copy; 2025 - Dibuat spesial untuk Hari Ibu
    </footer>

    <script>
        function bukaKado() {
            // Sembunyikan Overlay
            const overlay = document.getElementById('overlay');
            overlay.style.opacity = '0';
            overlay.style.visibility = 'hidden';

            // Tampilkan konten dengan animasi
            const content = document.getElementById('albumContent');
            content.classList.add('show-content');
        }
    </script>

</body>
