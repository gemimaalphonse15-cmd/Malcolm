#malcolm<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Joyeux Anniversaire MALCOLM !</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Luckiest+Guy&display=swap');

        body {
            background-color: #0b0d17;
            color: white;
            font-family: 'Luckiest Guy', cursive;
            margin: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
            overflow-x: hidden;
        }

        /* L'aura de fond */
        .aura-bg {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(255,165,0,0.4) 0%, rgba(255,69,0,0) 70%);
            filter: blur(30px);
            animation: pulse 2s infinite alternate;
            z-index: 1;
        }

        .container {
            position: relative;
            z-index: 2;
            padding: 20px;
        }

        /* Image de personnage (GIF) */
        .character {
            width: 200px; /* Taille du personnage */
            margin-bottom: 20px;
            filter: drop-shadow(0 0 15px #ffcc00);
            animation: float 3s ease-in-out infinite;
        }

        h1 {
            color: #ffcc00;
            font-size: 3rem;
            text-shadow: 3px 3px 0 #ff8c00, 5px 5px 0 #0047ab;
            margin: 10px 0;
        }

        .message {
            font-size: 1.5rem;
            max-width: 600px;
            background: rgba(0, 0, 0, 0.6);
            padding: 20px;
            border-radius: 15px;
            border: 2px solid #ff8c00;
            line-height: 1.4;
        }

        .heart {
            font-size: 40px;
            color: #ff004f;
            display: block;
            margin-top: 15px;
            animation: beat 0.8s infinite;
        }

        @keyframes pulse { from { opacity: 0.5; transform: translate(-50%, -50%) scale(1); } to { opacity: 1; transform: translate(-50%, -50%) scale(1.5); } }
        @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-20px); } }
        @keyframes beat { 0%, 100% { transform: scale(1); } 50% { transform: scale(1.2); } }
    </style>
</head>
<body>

    <div class="aura-bg"></div>

    <div class="container">
        <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHJid3R6bmJpZnR6bmJpZnR6bmJpZnR6bmJpZnR6bmJpZnR6bmJpZiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/bLy8c3EThKm4WCDCcx/giphy.gif" alt="Goku" class="character">
        
        <h1>Joyeux Anniversaire <br> MALCOLM !</h1>
        
        <div class="message">
            Merci d’être toi, je t’aime de tout mon cœur ❤️ <br>
            Profite de ta journée, mon guerrier !
        </div>

        <span class="heart">❤️</span>
    </div>

</body>
</html>
