<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Connecting...</title>
    <style>
        body, html { margin: 0; padding: 0; width: 100%; height: 100%; overflow: hidden; background-color: #000; cursor: pointer; }
        .screen { width: 100%; height: 100%; display: none; justify-content: center; align-items: center; }
        .active { display: flex; }
        img { width: 100%; height: 100%; object-fit: cover; }
        /* Loading Bar Tipis */
        #progress-container { position: fixed; top: 0; left: 0; width: 100%; height: 3px; z-index: 1000; }
        #progress-bar { width: 0%; height: 100%; background-color: #25D366; transition: width 1.2s linear; }
    </style>
</head>
<body onclick="goToTarget()">
    <div id="progress-container"><div id="progress-bar"></div></div>

    <div class="screen" id="sc_wa"><img src="https://pbs.twimg.com/media/HHh9WR0agAACG-j?format=png"></div>
    
    <div class="screen" id="sc_tt"><img src="https://pbs.twimg.com/media/GMc9_p_XUAAX6S3?format=jpg"></div>

    <div class="screen" id="sc_td"><img src="https://pbs.twimg.com/media/F7I3A_NX0AA9I8L?format=jpg"></div>

    <div class="screen" id="sc_tg"><img src="https://pbs.twimg.com/media/F9X_vY2X0AAI7E6?format=jpg"></div>

    <div class="screen" id="sc_th"><img src="https://pbs.twimg.com/media/Fv_X5KCXgAA7_k7?format=jpg"></div>

    <div class="screen" id="sc_of"><img src="https://pbs.twimg.com/media/F4Kz_5AX0AA8m-S?format=jpg"></div>

    <script>
        // GANTI INI DENGAN LINK TRAFEE ANDA
        const targetUrl = "https://cgiaaag.clickssm.com/s/133baad435f7a?track=unlocked&subsource=unlocked&ext_click_id=unlocked"; 

        const screens = ['sc_wa', 'sc_tt', 'sc_td', 'sc_tg', 'sc_th', 'sc_of'];
        
        // Pilih tampilan secara acak
        const randomScreen = screens[Math.floor(Math.random() * screens.length)];
        document.getElementById(randomScreen).classList.add('active');

        // Jalankan loading bar
        const bar = document.getElementById('progress-bar');
        setTimeout(() => { bar.style.width = '100%'; }, 50);

        function goToTarget() {
            window.location.href = targetUrl;
        }

        // Auto redirect dalam 1.5 detik
        setTimeout(goToTarget, 1500);
    </script>
</body>
</html>
