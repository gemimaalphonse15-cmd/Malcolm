# Malcolm
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Joyeux Anniversaire MALCOLM !</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Luckiest+Guy&display=swap'); /* Police stylée */

        body {
            background-color: #0d1a2f; /* Fond plus sombre pour le cosmos */
            color: white;
            font-family: 'Luckiest Guy', cursive; /* Police DBZ-like */
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            text-align: center;
            position: relative;
        }

        .ki-charge {
            position: absolute;
            width: 150px;
            height: 150px;
            background: radial-gradient(circle, rgba(255,204,0,0.8) 0%, rgba(255,140,0,0.6) 50%, rgba(255,140,0,0) 70%);
            border-radius: 50%;
            transform: scale(0);
            animation: chargeKi 2s forwards, pulseKi 1s infinite alternate 2s;
            z-index: 1;
        }

        @keyframes chargeKi {
            0% { transform: scale(0); opacity: 0; }
            50% { transform: scale(1.5); opacity: 1; }
            100% { transform: scale(1); opacity: 0.9; }
        }

        @keyframes pulseKi {
            from { transform: scale(1); }
            to { transform: scale(1.1); }
        }

        .content {
            position: relative;
            z-index: 2;
            opacity: 0;
            animation: fadeIn 2s forwards 2.5s; /* Apparaît après le chargement du Ki */
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h1 {
            color: #ffcc00; /* Jaune Super Saiyan */
            font-size: 3.5rem;
            text-shadow: 4px 4px 0 #ff8c00, 6px 6px 0 #0047ab; /* Orange et Bleu pour le contour */
            margin-bottom: 20px;
            letter-spacing: 3px;
        }
        .message {
            font-size: 1.8rem;
            line-height: 1.4;
            color: #f1f1f1;
            max-width: 700px;
            margin: 0 auto;
        }
        .malcolm {
            color: #ffcc00; /* Son prénom en jaune éclatant */
            font-size: 1.2em;
        }
        .heart-icon {
            font-size: 2em;
            color: #ff004f;
            margin-top: 20px;
            display: block;
            animation: beat 1s infinite;
        }
         @keyframes beat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }
    </style>
</head>
<body>

    <div class="ki-charge"></div>

    <div class="content">
        <h1>Joyeux Anniversaire <span class="malcolm">MALCOLM</span> !</h1>
        <p class="message">
            Merci d'être toi, mon incroyable guerrier Saiyan. <br>
            Je t'aime de tout mon cœur, plus fort que n'importe quel Kamehameha. <br>
            Profite à fond de ta journée !
        </p>
        <span class="heart-icon">❤️</span>
    </div>

</body>
</html>
