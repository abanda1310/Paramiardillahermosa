<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #000000, #1a1a2e);
            color: #ffd700;
            font-family: 'Arial', sans-serif;
            text-align: center;
            overflow: hidden;
        }
        .container {
            position: relative;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        h1 {
            font-size: 3em;
            margin-bottom: 1em;
            animation: fadeIn 3s ease-in;
        }
        p {
            font-size: 1.5em;
            margin: 0 20px;
            max-width: 700px;
            animation: fadeIn 4s ease-in;
        }
        .flowers {
            position: absolute;
            bottom: 0;
            display: flex;
            justify-content: center;
            align-items: flex-end;
            width: 100%;
        }
        .flower {
            animation: float 3s ease-in-out infinite, fadeIn 2s ease-in;
            margin: 0 10px;
        }
        .flower:nth-child(2) {
            animation-delay: 1s, 0.5s;
        }
        .flower:nth-child(3) {
            animation-delay: 2s, 1s;
        }
        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-20px);
            }
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
        .button-container {
            margin-top: 20px;
        }
        button {
            font-size: 1.5em;
            padding: 10px 20px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
        }
        .yes {
            background-color: #ff4d6d;
            color: white;
        }
        .no {
            background-color: #ccc;
            color: black;
        }
        .yes:hover {
            background-color: #e63950;
        }
        .no:hover {
            background-color: #aaa;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>¿Quieres ser mi San Valentín? ❤</h1>
        <p>Eres lo más hermoso que me ha pasado en la vida. Cada día contigo es un regalo, y no puedo imaginar este San Valentín sin ti a mi lado. 💖</p>
        <div class="button-container">
            <button class="yes" onclick="alert('Encontré una persona que es como mi canción favorita y la verdad que me encantaría escucharla por el resto de mi vida. Esa canción eres tú, mi amor. 💖')">Sí</button>
            <button class="no" onclick="alert('Oh... 💔 Pero siempre serás especial para mí.')">No</button>
        </div>
        <div class="flowers">
            <img class="flower" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/Flower_icon_-_yellow.svg/1024px-Flower_icon_-_yellow.svg.png" alt="Flor Amarilla" width="100">
            <img class="flower" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/Flower_icon_-_yellow.svg/1024px-Flower_icon_-_yellow.svg.png" alt="Flor Amarilla" width="120">
            <img class="flower" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/Flower_icon_-_yellow.svg/1024px-Flower_icon_-_yellow.svg.png" alt="Flor Amarilla" width="100">
        </div>
    </div>
</body>
</html>
