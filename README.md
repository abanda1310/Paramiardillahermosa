<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Serás mi San Valentín?</title>
    <style>
        body {
            background: linear-gradient(to right, #ff9a9e, #fad0c4);
            text-align: center;
            font-family: 'Arial', sans-serif;
            color: white;
            overflow: hidden;
        }
        h1 {
            font-size: 3rem;
            margin-top: 50px;
            animation: fadeIn 2s ease-in-out;
        }
        .heart {
            font-size: 4rem;
            animation: bounce 1s infinite;
        }
        .message {
            font-size: 1.5rem;
            margin: 20px;
            opacity: 0;
            animation: fadeIn 2s ease-in-out forwards;
        }
        .container {
            position: absolute;
            bottom: 50px;
            left: 50%;
            transform: translateX(-50%);
        }
        button {
            background: #ff4b5c;
            color: white;
            font-size: 1.5rem;
            padding: 10px 20px;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            transition: 0.3s;
        }
        button:hover {
            background: #ff1e42;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
    </style>
</head>
<body>
    <h1>💖 ¿Serás mi San Valentín? 💖</h1>
    <div class="heart">❤️</div>
    <p class="message" style="animation-delay: 1s;">Eres la razón por la que mi corazón late más fuerte.</p>
    <p class="message" style="animation-delay: 2s;">Cada día a tu lado es un regalo maravilloso.</p>
    <p class="message" style="animation-delay: 3s;">No imagino este día sin ti. 💕</p>
    <div class="container">
        <button onclick="respuesta(true)">¡Sí, quiero! 💘</button>
        <button onclick="respuesta(false)">Lo pensaré... 🤔</button>
    </div>
    <script>
        function respuesta(acepta) {
            if (acepta) {
                alert("¡Me haces la persona más feliz del mundo! 💞");
            } else {
                alert("Aún así, seguirás siendo mi persona especial. 💖");
            }
        }
        document.querySelectorAll('.message').forEach((el, i) => {
            setTimeout(() => { el.style.opacity = '1'; }, i * 1000);
        });
    </script>
</body>
</html>
